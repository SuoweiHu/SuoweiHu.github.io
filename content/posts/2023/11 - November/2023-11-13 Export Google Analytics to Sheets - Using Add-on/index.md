---
title: Export Google Analytics to Google Sheets (using Add-on)
date: 2023-11-13
tags: ["#Other"]
---


## Step-1 : Google Account Logged-in
To begin with, make sure you are **logged in** the proper google account, we will use the same account for all of the Google related product in the upcoming steps, including "Other" and "Google Sheets".

## Step-2: Install Add-on
Secondly, with the same google account open "google sheet", then open "`extension > add-on > get add-on"` and install the google analytics add-on as denoted in the screenshot:

![2023.11.13 - 132915](2023.11.13%20-%20132915.jpg)

## Step-3: Create, Configure, Generate Report
Once you have the extension installed, you can proceed to "`extension > google analytics > create report`" to create a new report exportation configuration, in this configuration sheet, you can select the parameter for export, the main focus are: "start/end date", "metrics exporting", "dimensions exporting", and "limit" (number of record, recommended to be less than 1000'0000)

![2023.11.13 - 133746](2023.11.13%20-%20133746.jpg)

For example here we have:
```
Start Date:	    2020-08-01
End Date:	    2023-11-01
Metrics:	    ga:entrances,ga:pageviews,ga:uniquePageviews,ga:avgTimeOnPage,ga:exits
Dimensions:	    ga:pagePath,ga:date
Limit:	            1000
```

Once you have all the parameter configured, you can proceed to the menu bar and generate the report via "`extension > google analytics > run reports`", which will give you something looks like the following screenshot shows; Note that only partial of the data are valid entries (here "`A15:G1015`"), so be mindful of this valid range when you are about to import data to stuff like Google Looker.


![2023.11.13 - 134039](2023.11.13%20-%20134039.jpg)

---
**Reference**
- [Google Analytics Spreadsheet Add-on](https://developers.google.com/analytics/solutions/google-analytics-spreadsheet-add-on)
- [How to backup Universal Analytics: Exporting data from Google Analytics and moving to GA4](https://youtu.be/WGIe_HgIdBg?si=8Z6IWZ-XEMi0_nKY)