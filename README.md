# Citi Bike Analysis

> Breakdown of Citi Bike's rider data in New York City from August 2019 for insights into bike usage in 2020.

![citi-bikes](resources/citi-bike.jpg)

## Overview of Project

This current repo is a playing with data from Citi Bike Trip Histories. I've made several charts and graphs and we now know the breakdown of rider types in New York City. We know this by the first round of data analysis we did [Citi Bike Analysis Tableau](https://public.tableau.com/profile/jovanipink#!/vizhome/BikeSharing_16039941514670/CitiBikeDashboard) which is feeding to my greater final analysis on User Type and COVID []().

I've also charted Citi Bike's data dump sizes and times: [Profiling Citi Bike Trip Data](https://public.tableau.com/profile/jovanipink#!/vizhome/ProfilingCitiBikeTripData/FileSize)

## Folder Structure

```
src/
├── data
│ ├── external
│ ├── interim
│ ├── processed
│ │ └── NYC_Citibike_Processed_Data.csv
│ └── raw
│ └── 201908-citibike-tripdata.csv
├── reports
│ └── powerbi
│ └── nyc-citibike.pbix
├── resources
├── .gitignore
├── LICENSE.md
├── nyc-citibike.ipynb
└── README.md
```

## Analysis

We pulled Citi Bike's data using Python and Pandas to verify the available download sources, data modified, and size. Once we've cleaned up the raw data we did further analysis and visualization in Tableau. We started asking questions of the data on understanding Citi Bike's business, questions that would gve us insights in finding out the ride sharing number during the pandemic.

Originally I was fixed on Gender [Citi Bike Analysis Gender](https://public.tableau.com/profile/jovanipink#!/vizhome/NYCCitibike_16041943647530/Location) and bike usage and concluded that the majority of every category are male. Ok.

When further digging into the dataset one particular column (field) "User Type" caught my attention because of what it "could" say about the rider. The user type is either a customer or subscriber so that customer made the decision of being part of one of those three options.

- Customer = 24-hour pass or 3-day pass user
- Subscriber = Annual Member

Further looking into the details of User Type from Citi Bike's website:

Subscriber:

- https://www.citibikenyc.com/pricing/annual

Customer:

- https://www.citibikenyc.com/pricing/day
- https://www.citibikenyc.com/pricing/single-ride

I wanted to see what the behavior pattern were for both types and their ride usage during the pandemic.

### Resources

Data sources are CSV files provided by [Citi Bike](https://www.citibikenyc.com/system-data) that lead you to their [Citi Bike Data download page](https://s3.amazonaws.com/tripdata/index.html).

The CSV file below is the data set used in the initial analysis project...

|               Name               |       Date Modified        |   Size    |   Type   |
| :------------------------------: | :------------------------: | :-------: | :------: |
| 201908-citibike-tripdata.csv.zip | Sep 18th 2019, 01:33:14 pm | 100.02 MB | ZIP file |

Analytic Visualization tool we used is Tableau Desktop: https://public.tableau.com/s/

The Data profile:

- Trip Duration (seconds)
- Start Time and Date
- Stop Time and Date
- Start Station Name
- End Station Name
- Station ID
- Station Lat/Long
- Bike ID
- User Type (Customer = 24-hour pass or 3-day pass user; Subscriber = Annual Member)
- Gender (Zero=unknown; 1=male; 2=female)
- Year of Birth

#### Results

The following questions were answered about the data using Tableau:

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

We went on to download all the datasets from January 2018 to January 2021

:)

## Todo Checklist

A helpful checklist to gauge how your README is coming on what I would like to finish:

- [ ] Fix and Update the styling of the Dashboards and Stories.
- [ ] Redo everything in Power BI.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

1. Fork this repository;
2. Create your branch: `git checkout -b my-new-feature`;
3. Commit your changes: `git commit -m 'Add some feature'`;
4. Push to the branch: `git push origin my-new-feature`.

**After your pull request is merged**, you can safely delete your branch.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for more information.
