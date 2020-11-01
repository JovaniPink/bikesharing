# NYC BikeSharing

> Breakdown of Citi Bike's rider data in New York City in August 2019.

![citi-bikes](resources/citi-bike.jpg)

## Overview of Project

We now know the breakdown of rider types in New York City, which will help us predict the customer breakdown in Des Moines and, in turn, propose a business model to investors. We know this by the first round of analysis we did [BikeSharing](https://public.tableau.com/profile/jovani.pink#!/vizhome/BikeSharing_16039941514670/NYCCitiBikeDashboard?publish=yes) and then in our final analysis [NYC Citi Bike](https://public.tableau.com/profile/jovani.pink#!/vizhome/NYCCitibike_16041943647530/PredominantlyMaleClients?publish=yes).

## Summary

We pulled Citi Bike's data and with Tableau and started asking questions of the data and asked questions of what information should we convey to investors.

### Resources

Analytic Visualization tool we used is Tableau: https://public.tableau.com/s/

Data source:
The CSV file below is the data set used in this project. They are from the [Citi Bike Data download](https://s3.amazonaws.com/tripdata/index.html) webpage.

|               Name               |       Date Modified        |   Size    |   Type   |
| :------------------------------: | :------------------------: | :-------: | :------: |
| 201908-citibike-tripdata.csv.zip | Sep 18th 2019, 01:33:14 pm | 100.02 MB | ZIP file |

### Results / Analysis

You've answered two questions about the data using Tableau:

How many bike trips were recorded during the month of August?

![NumbersOfRides](resources/NumbersOfRides.png)

We'll figure out the peak hours for bike trips during the month of August. This will help our investors get a ballpark estimate of how many bikes we might need in Des Moines. What Are Peak Riding Hours in the Month of August?

![AugustPeakHours](resources/AugustPeakHours.png)

What are the highest-traffic locations? Understanding both when and where people use Citi Bike will help you plan your pilot in Des Moines.

![TopStartingLocations](resources/TopStartingLocations.png)

What can the data tell us about the riders themselves? Often, the first place we start when understanding a population is gender.

![GenderBreakdown](resources/GenderBreakdown.png)

While working with the data we found that the majority of clients were men.

![AgeGroup](resources/AgeGroup.png)

## Folder Structure

src/
├── data
│ ├── interim
│ ├── processed
│ │ └── NYC_Citibike_Processed_Data.csv
│ └── raw
│   └── 201908-citibike-tripdata.csv
├── reports
├── resources
├── .gitignore
├── LICENSE
├── nyc-citibike-challenge.ipynb
└── README.md

## Todo Checklist

A helpful checklist to gauge how your README is coming on what I would like to finish:

- [ ] Fix and Update the styling of the Dashboards and Stories.
- [ ] Redo everything in Power BI.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
