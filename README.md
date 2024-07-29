# python-api-challenge
Data Analytics Boot Camp Module 6 Challenge

## Contents
- **WeatherPy/api_keys.py**: You will need to provide this file with your API keys.
- **WeatherPy-starter.ipynb**: Starter notebook for the VacationPy portion of the challenge
- **WeatherPy-RPM.ipynb**: My solution to the VacationPy portion of the challenge
- **VacationPy-starter.ipynb**: Starter notebook for the VacationPy portion of the challenge
- **VacationPy-RPM.ipynb**: My solution to the VacationPy portion of the challenge

## Instructions
- To run the WeatherPy notebook, you may need to install citipy ("pip install citipy" before launching Notebook)
- To run the VacationPy notebook, you must first run the WeatherPy notebook to generate the necessary files
- To run the VacationPy notebook, you must also run Notebook in an environment set up like hvplot-env in the bootcamp activity files

## Notes
The WeatherPy starter notebook has a simple exception handler treating ANY exception from the request and parsing of city data as though it means the city wasn't found. This is a terrible pattern to teach people. Exceptions happen for lots of reasons, in my case usually because I wasn't digging into the JSON structure right. The correct way to detect a "city not found" error is by looking at the response code: 404 means Not Found.