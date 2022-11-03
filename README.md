<img width="250" src="https://raw.githubusercontent.com/lukwies/mid-bootcamp-project/main/data/img/bikes.png">


# Bikesharing in Seoul (South Corea)

Rental bikes are currently introduced in many urban cities for the enhancement of mobility comfort.
It is important to make the rental bike available and accessible to the public at the right time as
it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes
eventually becomes a major concern.
The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. 
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint,
Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
For a detailed description of the dataset, [click here](#Data-Attributes).


## Business Questions

So let's assume we are working for a company in Seoul which provides rental bikes and wants
us to find answers for the following business questions:

    * What impact has the season (Spring, Summer, Autumn, Winter) on bike renting?
    * How big is the amount of rented bikes at different times during the day?
    * Does the amount differ between workdays, weekends and holidays?
    * What impact does the weather (temperature, rain, snow, ...) have on bike renting?
    * Under what conditions is the rental the highest/lowest?

## Hypothesis Testing

We also want to verify some hypothesis our chief was claiming.

     1. The daily rental amount differs from 400 bikes/hour.
     2. We have a higher rental amount during holidays.
     3. The average rental amount is less if the weather is cold (< 10°C)
     4. The average rental amount is higher during the day (8°°-19°°) than at night.

All hypothesis tests can be found 
<a href='https://github.com/lukwies/mid-bootcamp-project/blob/main/notebooks/hypothesis_test.ipynb'>
here</a>.

## Prediction

    * Can we predict the amount of bikes rented for any given day/hour?

The code for predicting the rental amount can be found
<a href='https://github.com/lukwies/mid-bootcamp-project/blob/main/notebooks/hypothesis_test.ipynb'>
here</a>.

## Data Attributes

<pre>
  Date - year-month-day
  Rented Bike count - Count of bikes rented at each hour
  Hour - Hour of he day
  Temperature-Temperature in Celsius
  Humidity - %
  Windspeed - m/s
  Visibility - 10m
  Dew point temperature - Celsius
  Solar radiation - MJ/m2
  Rainfall - mm
  Snowfall - cm
  Seasons - Winter, Spring, Summer, Autumn
  Holiday - Holiday/No holiday
  Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)
</pre>

The (uncleaned) raw data file can be found 
<a href='https://github.com/lukwies/mid-bootcamp-project/blob/main/data/raw/bike_rentals.csv'>
here</a>.

## Sources
 * Data: https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand
 * Image: https://global.chinadaily.com.cn/a/201801/25/WS5a69cab3a3106e7dcc136a6d.html

## Conclusions
	* The highest rental amount can be found in june on fridays around 6:00pm when the temperature is ~27°C.
	* The result of the hypothesis tests was 1=False, 2=False, 3=True, 4=True

