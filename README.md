# Weather App

Weather App

A simple but powerful weather app that provides real-time weather information and forecasts for any location in the world.

#Features:

#The application allows users to search for the weather conditions in a specific location.
#The application displays the selected location's current weather conditions, temperature, and humidity.
#The application has a responsive user interface that works on both desktop and mobile devices.
#The application uses an API to retrieve weather data.
#The application is built using a front-end framework such as React and a back-end framework such as Django.

## How to use

Enter any location in the world and it should display a weather card containing the following information :

- Temperature
- Humidity
- Weather Description

## External APIs Used

- OpenWeather Geocoder API: To retrieve the latitude and longitude of a location
- OpenWeather Current Weather API: To retrieve the weather information for that location

## Dependancy

This project consists of a frontend React application and a backend Django server. The dependencies for each are listed below:

#### Frontend

- React
- react-dom
- react-scripts
- @mui/material

#### Backend

- Django
- requests
- python-dotenv

## Run on local machine

#### 1. Clone the git repository

```bash
git clone https://github.com/saurzv/weather-app.git
```

#### 2. Install required packages for backend and frontend and run servers

Go to the _server_ directory

```bash
cd weather-app/server/
```

And run

```bash
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

This will install all the required packages for the backend.

Create a .env file and paste your OpenWeather API as

```
API_KEY=<YOUR_API_KEY>
```

Make migrations and start the backend server

```bash
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver localhost:8000
```

Similarly for frontend

```bash
cd weather-app/client/
yarn
```

or

```bash
cd weather-app/client/
npm install
```

After installing the required packages, start the frontend server

```bash
yarn start
```

or

```bash
npm start
```

The site should start running
