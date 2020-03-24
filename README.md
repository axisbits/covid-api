# covid-api
Public API for Covid-19 data by Johns Hopkins CSSE https://github.com/CSSEGISandData/COVID-19. 

#### Website - https://covid-api.com
#### Documentation - https://covid-api.com/api

# Important

As for the data structure [update](https://github.com/CSSEGISandData/COVID-19/issues/1250), we need some time to rewrite the processing logic. Will be done today, 2020-03-24.

# Change log

## 2020-03-23

1. "mortality" changed to "fatality_rate", as was suggested by [ezanardi](https://github.com/ezanardi)

## 2020-03-19

1. Added "mortality" = deaths / confirmed, as was suggested by [impredicative](https://github.com/impredicative)

## 2020-03-18

1. Added "active" and "active-diff" (active = confirmed - deaths - recovered) as was suggested by [impredicative](https://github.com/impredicative)

## 2020-03-16

1. Added ISO codes for countries
2. Added statistics diff with the previous day