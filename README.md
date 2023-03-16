# Important
On March 10, 2023, Johns Hopkins CSSE stopped publishing data on Covid statistics on their GitHub Repository. 
This API continues to provide historical data until March 10. 2023, but no new data will be available.
# covid-api
Public API for Covid-19 data by Johns Hopkins CSSE https://github.com/CSSEGISandData/COVID-19. 

#### Website - https://covid-api.com
#### Documentation - https://covid-api.com/api

# Changelog

## 2021-04-09

1. Added optional parameters of sorting and pagination to /regions and /provinces endpoints.
2. Added optional parameters of sorting and pagination of regions to the /reports endpoint.
3. Added optional filter by ISO to the /reports/total endpoint. Please note that the calculation is done as a sum of statistic numbers across all regions within the country that may include overseas and dependent territories.

## 2020-04-22

1. Added filter by city_name to /reports endpoint. Note that currently city data is available for the USA only.

## 2020-04-17

1. Changed /reports/total query parameters - "date" is now optional. If not provided, the data for the latest date will be returned.

## 2020-04-15

1. Added following fields to the /reports/total endpoint: 
    - date
    - last_update
    - recovered
    - recovered_diff
    - active
    - active_diff
    - fatality_rate 

## 2020-04-08

1. Added new endpoint - total data for the entire world for particular date, as was suggested by [mgfcf](https://github.com/mgfcf). Example - https://covid-api.com/api/reports/total?date=2020-04-07. 


## 2020-03-26

1. Added confirmed and deaths data for the US cities. Arrays of cities are added to each state. 
2. Data for recovered cases for US and Canada cases at the state/province level is consolidated under a province named "Recovered". This is because Johns Hopkins CSSE does not update it at the state/province level for US and Canada. For all other countries and territories, this data is still present.

## 2020-03-23
  
1. "mortality" changed to "fatality_rate", as was suggested by [ezanardi](https://github.com/ezanardi)

## 2020-03-19

1. Added "mortality" = deaths / confirmed, as was suggested by [impredicative](https://github.com/impredicative)

## 2020-03-18

1. Added "active" and "active-diff" (active = confirmed - deaths - recovered) as was suggested by [impredicative](https://github.com/impredicative)

## 2020-03-16

1. Added ISO codes for countries
2. Added statistics diff with the previous day