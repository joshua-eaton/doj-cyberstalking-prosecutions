# doj-cyberstalking-prosecutions

This repository contains data on federal prosecutions under [18 USC 2261a(2)](https://www.law.cornell.edu/uscode/text/18/2261A) (the federal cyberstalking statute) and [18 USC 875(c)](https://www.law.cornell.edu/uscode/text/18/875) (the federal online harassment statute) for FY 2012 – FY 2017. The Executive Office for Unites States Attorneys, a unit of the Department of Justice, provided this data to ThinkProgress in 2017 in response to two Freedom of Information Act requests. 

The data comes from the United States Attorneys' Case Management System. The Department of Justice provided it in two PDF tables (see [here](https://www.documentcloud.org/documents/4047304-Eaton-Letter-1.html) and [here](https://www.documentcloud.org/documents/4049303-Eaton-Letter-2-2.html)). To get that data into a workable format, I took the following steps:
* I manually recreated those two tables in separate sheets in a Google Sheets workbook,
* compared the two PDFs with the two spread sheets to check for data-entry errors,
* used a SUM formula to add a "subtotal" row to both sheets for FY 2012 – FY 2016,
* used the same SUM formula to create a third sheet that combines the totals for both 18 USC 875(c) and 18 USC 2261a(2) for FY 2012 – FY 2016 (explanation for why I left out FY 2017 is below), and
* exported the three resulting spread sheets into three CSV files.

Here's a breakdown of what's in each of the three CSV files that came out the end of this process:

* [Both 18 USC 875(c) and 18 USC 2261a(2) data, FY 2012 - FY 2016.csv](https://github.com/joshua-eaton/doj-cyberstalking-prosecutions/blob/master/Both%2018%20USC%20875(c)%20and%2018%20USC%202261a(2)%20data%2C%20FY%202012%20-%20FY%202016.csv) — This file contains data on federal prosecutions under **both** 18 USC 875(c) **and** 18 USC 2261a(2) from the beginning of FY 2012 (Oct. 1, 2011) through the end of FY 2016 (Sept. 30, 2016). I did not include any FY 2017 data in this file because that data stops at a different date for each charge (see below).
* [Just 18 USC 2261a(2) data, FY 2012 - FY 2017.csv](https://github.com/joshua-eaton/doj-cyberstalking-prosecutions/blob/master/Just%2018%20USC%202261a(2)%20data%2C%20FY%202012%20-%20FY%202017.csv) — This file contains data on federal prosecutions under **just** 18 USC 2261a(2) from the beginning of FY 2012 (Oct. 1, 2011) through Jan. 31, 2017. So the FY 2017 data is incomplete. 
* [Just 18 USC 875(c) data, FY 2012 - FY 2017.csv](https://github.com/joshua-eaton/doj-cyberstalking-prosecutions/blob/master/Just%2018%20USC%20875(c)%20data%2C%20FY%202012%20-%20FY%202017.csv) — This file contains data on federal prosecutions under **just** 18 USC 875(c) from the beginning of FY 2012 (Oct. 1, 2011) through Nov. 30, 2016. So the FY 2017 data is incomplete.

Some things to keep in mind when looking at this data:
* It only includes cases in which 18 USC 875(c) and/or 18 USC 2261a(2) were the first charge on the indictment.
* It only includes cases in which DOJ staff entered the specific subsection (for example, 18 USC 2261a(2)) rather than the main statute (for example, 18 USC 2261a).
* All dates are based on the federal fiscal year, which runs from Oct. 1 of the previous calendar year through Sept. 30. In other words, FY 2012 began on Oct. 1, 2011, and ended on Sept. 30, 2012.
