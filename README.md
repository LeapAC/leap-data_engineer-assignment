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
  - There may be gaps in the input time series -- there should _not_ be gaps in the output time series.
  - You do not have to interpolate or otherwise fill in the missing `energy_wh` values, but can if you wish to
- The CSV file should include the following additional data fields: 
  - The average energy usage per hour 
  - a (True/False) flag indicating missing intervals -- where the missing data/gaps have been filled.

Other notes: 
- The solution should only include native PySpark (no UDFs or UDAFs please).
- The hourly average is per a specific hour and should be per the start of hour (clock-hour), not rolling. 
- The solution should be a generic solution for this problem and not tailored to the data provided. 
  - For example, this solution should be able to work with megabytes _or_ terabytes of data.
  - In production, this solution would be used on millions of rows -- please provide a solution that will scale.
- Please provide a python file that can be run to generate the output as part of your solution.


If you have any questions at all, please don't hesitate to e-mail Marco with them. 

We are looking forward to your solution!

