# python-api-challenge
---
## WeatherPy
In the first part of weatherpy I created plots to display the relationship between weather variables (temperature, humidity, cloudiness, and wind speed) and latitude

### Latitude vs. Temperature
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/ba05eafc-9553-4b39-a796-f1bc615ec86c)

### Latitude vs. Humidity
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/16eaa108-c0cd-424b-bb2f-a6c18323a7b7)

### Latitude vs. Cloudiness
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/d45d78d2-745f-4ef7-9486-d8670558c8fa)

### Latitude vs. Wind Speed
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/45136f5b-8199-4a77-871e-7b9ffcb69423)
----
#### For the second part of weatherpy I computed liner regression for each relationship in both the Northern and Southern Hemisphere

## Latitude vs. Temperature - Linear Regression Line
#### Northern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/104feafe-7a92-4b2c-89f7-4678d04a3911)

#### Southern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/aba8751d-5ac5-4482-8486-48d6b980a900)

## Latitude vs. Humidity - Linear Regression Line
#### Northern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/27edadd9-bd79-41ae-8a87-1541c3c4ad3b)

#### Southern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/ab5b1073-3251-4f70-b45e-170e53ca5830)

## Latitude vs. Cloudiness - Linear Regression Line
#### Northern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/7f88bbd2-16bb-4cae-9fbc-ee97e23feb95)

#### Southern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/b4a22d9e-f9ac-46f0-879e-c133847a9b34)

## Latitude vs. Wind Speed - Linear Regression Line
#### Northern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/06fe4558-df75-4ab8-b246-ceab1defbc28)

#### Southern Hemisphere
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/2fd16f44-4b63-4c4a-b6eb-e161ae44534c)
---
## VacationPy
For VacationPy I used a Geoapify API key to display a map visualization for every city in the city_data_df. Then I narrowed down the data to US cities that have zero cloudiness and a wind speed less than 4 m/s.
```
city_data_df = city_data_df[(city_data_df["Cloudiness"] == 0)]
city_data_df = city_data_df[(city_data_df["Country"] == "US")]
city_data_df = city_data_df[(city_data_df["Wind Speed"] < 4)]
```
Then I created a new dataframe to store the city, country, coordinates, and humidity.  After that, I used the Geoapify API to find the first hotel within 10,000 meters of my coordinates. 
![image](https://github.com/Faith-Hall/python-api-challenge/assets/135525815/6e67a208-4f65-453c-8beb-15c47bd3479c)
