# Introduction

You've been invited to complete this data engineering coding assignment. 

We have deliberately designed this assignment to be open-ended in order to leave plenty of room for you to make choices. 

Please document your Pyspark code.  We do not expect you to spend days on this nor to build a full-blown application.

Good luck!

-Leap.

## Assignment

In this repository you'll find a directory with files containing energy meter-data.

Please build a PySpark solution that does the following:
- It reads in the data 
- It writes out a file in CSV with the energy usage for each meter at each 15 minute interval. 
- The CSV file should include the following additional data fields: 
  - The hourly averaged energy usage (per clock-hour)
  - a (True/False) flag indicating missing intervals.  

Other notes: 
- The solution should only include native PySpark (No UDFs or UDAFs please).
- The hourly average should be per hour, not rolling.
- The solution should be a generic solution for this problem and not tailored to the data provided. 
  - For example, this solution should be able to work with megabytes _or_ a terabyte of data.
- In production, this solution would be used on millions of rows -- please provide a solution that will scale.


Please provide your Pyspark code to this assignment. We are looking forward to your solution!

