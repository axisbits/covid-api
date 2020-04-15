# covid-api
Public API for Covid-19 data by Johns Hopkins CSSE https://github.com/CSSEGISandData/COVID-19. 

#### Website - https://covid-api.com
#### Documentation - https://covid-api.com/api

# Change log

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