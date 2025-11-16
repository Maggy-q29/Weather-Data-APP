**Weather Data in Power BI** 

**This project shows how to connect Power BI to the OpenWeather API to get real-time weather information for any city.**

API URL Used
https://api.openweathermap.org/data/2.5/weather?q={CITY}&appid={YOUR_API_KEY}&units=metric


Replace {CITY} with the city name and {YOUR_API_KEY} with your API key.

Steps to Use in Power BI

Get your API key

Sign up at https://openweathermap.org/

Copy your key.

Connect in Power BI

Open Power BI Desktop

Click Get Data → Web

Paste your full API link, for example:

https://api.openweathermap.org/data/2.5/weather?q=Nairobi&appid=YOUR_API_KEY&units=metric


Transform the JSON

Open Power Query

Expand the following fields:

main → temp, humidity, feels_like

weather → description

wind → speed

Rename columns as needed.

Load the data

Click Close & Apply to load the table into Power BI.

Example Data You Will Get

City name

Temperature (°C)

Weather description

Humidity

Wind speed

Optional: Use Parameters

You can create parameters in Power Query:

City Parameter

"https://api.openweathermap.org/data/2.5/weather?q=" & City & "&appid=" & APIKey & "&units=metric"


This makes it easy to change the city.
