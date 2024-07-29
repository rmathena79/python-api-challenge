# python-api-challenge
Data Analytics Boot Camp Module 6 Challenge

## Contents
- 
-
-

## Instructions
- pip install citipy
- set up hvplot-env as described in the activities
- Run the notebook to generate the output files

## Notes
The WeatherPy starter notebook has a simple exception handler treating ANY exception from the request and parsing of city data as though it means the city wasn't found. This is a terrible pattern to teach people. Exceptions happen for lots of reasons, in this case usually because we aren't digging into the JSON structure right. The correct way to detect a "city not found" error is by looking at the response code: 404 means not found.