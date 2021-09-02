# GitHub Actions instructions
## Overlapping issue with background jobs
The date of analysis cannot be older than the date of the last known analysis on this project. Value: "2021-08-30T19:30:38+0000". Latest analysis: "2021-08-30T19:30:54+0000". It's only possible to rebuild the past in chronological order.

Explanation:
Here is the scenario of what happened to you:

Two jobs doing an analysis of your project started nearly at the same time. Let's call them job A and B.

A starts at 11H20, B starts at 11H21.
Since A started before B, its analysis date (11H20) is before B (11H21) (thank you Captain obvious!)
**For some reason, B ends before A and submits the report first**. Then A finishes and submits its report as well.
We now have two reports for the same project in the queue : report B and report A (in order).
Report B is processed first (all tasks are processed in order of submission), the processing finishes and then the date of the most recent analysis of your project becomes 11H21 (the date of the analysis stored in report B).
Report A is then processed. Since analyses can only processed forward in time, a check exists (early in processing, that's why your second task lasted only a few ms) and fails in this case because the date of report A is 11H20, which is before the date of the current last analysis.

The date reported in the log is the analysis date.
Btw, Compute Engine is designed so that tasks for a given project can never be processed in parallel. So, this also applies with multiple workers.
