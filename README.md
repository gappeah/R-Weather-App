# Weather Activity Suggestion App

This is a simple command-line weather app written in R that provides activity suggestions based on the current weather conditions such as temperature, wind speed, rain status, cloudiness, and time of day.

## Features

- Takes user input for temperature, wind speed, rain status, cloudiness, and time of day.
- Offers varied suggestions for outdoor or indoor activities based on the weather.
- Custom responses for different temperature ranges, wind speeds, and rain conditions.
- Flexible activity recommendations, such as staying hydrated on hot days or flying kites on windy days.

## How It Works

The app uses basic `readline()` functions to prompt the user for the following inputs:

- **Temperature** (in Celsius)
- **Wind speed** (in km/h)
- **Rain status** (yes/no)
- **Cloudiness** (yes/no)
- **Time of day** (morning, afternoon, evening, night)

Based on the input, the app uses conditional logic to suggest various activities, such as:
- Staying indoors when it's too hot or cold
- Going for a walk or having a picnic on pleasant days
- Suggesting rain-friendly or windy-day activities like using an umbrella or flying a kite

## Installation

1. Make sure you have R installed on your machine. You can download it [here](https://www.r-project.org/).
2. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/gappeah/weather-app.git
   ```
3. Navigate to the app's directory:
   ```bash
   cd weather-app
   ```
4. Run the app in your R environment:
   ```r
   source("weather_app.R")
   ```

## Usage

When you run the app, it will prompt you to input the current weather details:

1. **Temperature**: Enter the current temperature in Celsius.
2. **Wind Speed**: Enter the current wind speed in km/h.
3. **Rain Status**: Respond with "yes" if it's raining or "no" if it's not.
4. **Cloudiness**: Respond with "yes" if it's cloudy or "no" if it's clear.
5. **Time of Day**: Enter the current time of day (morning, afternoon, evening, night).

Based on your inputs, the app will suggest an activity suited to the weather.

Example:
```bash
Please enter the current temperature (in Celsius): 25
Please enter the current wind speed (in km/h): 15
Is it currently raining? (yes/no): no
Is it cloudy? (yes/no): no
What time of day is it? (morning/afternoon/evening/night): afternoon

It's a beautiful day for outdoor activities like hiking or a picnic.
```

## Sample Data

The app also generates a small dataset of hypothetical weather conditions and corresponding activities as an example:

| Temperature | Wind Speed | Rain | Cloudy | Time of Day | Activity                              |
|-------------|------------|------|--------|-------------|---------------------------------------|
| 35          | 15         | no   | no     | afternoon   | Stay indoors and hydrate              |
| 25          | 25         | no   | yes    | morning     | Nice day for a hike or picnic         |
| 15          | 35         | yes  | no     | evening     | Chilly and windy, consider indoor activities |
| 5           | 45         | yes  | yes    | night       | Cold and windy, bundle up if outside  |
| -5          | 55         | no   | no     | afternoon   | Freezing! Stay warm indoors           |
