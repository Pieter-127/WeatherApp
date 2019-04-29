#Weather App
A simple proof of concept weather app made with kotlin and a variety of other android frameworks and principles, making use of dependency injection, MVVM and HTTP.

#Background
A lot of companies make use of a weather app as their evaluation for how skilled a developer is, so I thought it would be a good idea
to try my best at making a weather app with all the skills I've learned since starting my journey with kotlin.

This project makes use of Kotlin, Retrofit and GSON for the majority of the features : retrieving data from two different api's and
then populating the UI, which is built using constraint layout, glide and android standards for localization.

After the data from the api's are returned, I implemented some basic caching, making use of a Room database to store the results of requests,
which are then returned to the user when they launch the app again, to improve the UX a bit and also to learn some new skills with Room, RxJava and the idea of caching.

I made use of the MVVM architecture, as this is my favourite architecture to use and used Dagger for dependency injection, as this is
also an industry standard framework for android development.

I really learned a lot of things from this project, including retrofit and material design and this was a really fun, quick project to work on


# Overview
![Screenshot](art/overview.png)

# Libraries and Frameworks
- Kotlin
- Android Support Library
- Constraint layout
- Architecture components
- Dagger
- RxJava
- GSON
- Timber
- Glide
- Retrofit

# API's
- Openweather
- Apixu

# How the app works
- When the user opens the application, the application will prompt the user to turn on their gps and ensure that they have an internet connection.
- Once available, the application will collect the user's current location and make use of that to do several API calls to the different api's for information regarding the current weather, as well as a 7 day forecast
- The responses of these requests will be cached to ensure the user can still see the weather information previously gathered if they use the app with no internet connection in future
- The application will then show the user's address, a daily forecast of weather as well as to display an additional 7 day forecast and the status of the weather

# Attributions
- original design by Punit Chawla (https://www.uplabs.com/punitdesign)
- modifications and icon design by Roch (http://www.artroch.co.za/)

Source at private bitbucket, this is just as an overview of work done previously, feel free to send me a message and I'll make it available :) 
