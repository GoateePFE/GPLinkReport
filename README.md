# GPLinkReport

Courtesy of your friendly, neighborhood Microsoft PFE

Mr. Ashley McGlone

http://aka.ms/GoateePFE

This script creates a report of all group policy links, their locations, and
their configurations in the current domain, and their replication metadata
for auditing and forensics. Output can be piped to a CSV file, Out-Gridview,
etc.

tl;dr - It shows you where all of your GPOs are linked to the OUs and where
blocking or no-override is turned on. It also shows you forensics data like
when it was last linked or edited.

Call this script like this:
```
.\gPLinkReport.ps1 | Out-GridView
.\gPLinkReport.ps1 | Export-Csv -Path .\GPLinkReport.csv -NoTypeInformation
```
