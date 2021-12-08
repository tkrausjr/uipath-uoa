# Daily_UOA_BarChart_IBD_Analysis


Daily_UOA_Barchart_IBD_Analysis Project
This project will download Unusual Options Activity on a Daily Basis, filter out the highest Value New Options Trades and then cross Reference that list against Fundamentally superior stocks from an exisitng Database we maintain. Sending the results in an email each night.



1) Validate whether you are logged into Barchart.com website
2)If not, Login to barchart.com website or if so continue to next step
3) Navigate to Unusual Options Activity page
4) Download barchart-unusual-options-activity.csv & move to \Documents\UOA Workspace\barchart-data folder
5) Load "Z:\finance-analysis\ipython\daily-analysis\daily-uoa-analysis_uipath-python.py" Python Script
6) Call analyze: function in Python script
   NOTE: This script will filter out Highest Value New Trades, and Cross Reference against Fundamentally High Quality Stocks sending the merge of the two.
7) Get Function return JSON Array as String
8) Deserialize JSON Array to a DataTable
9) DEBUG - Print Datatable as String and Count Rows in Datatable
10) Transform DataTable into HTML
11) Send SMTP Email with results
