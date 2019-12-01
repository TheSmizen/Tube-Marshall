# TFL API notes

## Stuff:

### NaPTAN 
(we prefer NAPTAN - much easier)

NAPTAN is a dataset/system for identifying transit stops. gov.uk has a repository of them.
For example 'HUBLBG' is the NAPTAN ID for London Bridge.

https://data.gov.uk/dataset/ff93ffc1-6656-47d8-9155-85ea0b8f2251/national-public-transport-access-nodes-naptan
https://wiki.openstreetmap.org/wiki/NaPTAN

## How to routefind between two points:
GET	/Journey/JourneyResults/{from}/to/{to}
- Example URI:

https://api.tfl.gov.uk/Journey/JourneyResults/London%20Bridge%20Station/to/Earl's%20Court%20Station?nationalSearch=false&date=20191201&time=1650&timeIs=Departing&journeyPreference=LeastTime&mode=overground%2Ctube%2Cwalking&accessibilityPreference=NoRequirements


