# weather-forecast
------------------------------------------------------------------------------Markup of the App-------------------------------------------------------
The markup or HTML of the app is straightforward. You can see the image below of the final output to get an idea about our markup style.
We have an image that will change according to the weather. The location will be based on the user's geolocation. Below it is the summary of the weather, the temperature is in both Celcius and Fahrenheit. And in the end, we are showing the sunrise and sunset time. We are also using the Lora google font.
------------------------------------------------------------------------------js of the app-------------------------------------------------------Getting Data from API
The first thing to understand is how do we get the weather data? To get the data, we are dependent on a third-party service. We will use a website called OpenWeatherMap. OpenWeatherMap is a service that provides various weather data through API. We can integrate the API into our app and can use the data on our website. An API is like a waiter, it works as a medium between the server and the client to serve the data to the client according to the client's request.

OpenWeatherMap is free up to a certain number of requests. After that, it charges money. To use the API, we need an API key. Let's see how we can get our API key:

Step 1: Open OpenWeatherMap and click on Sign In:Step 2: Click on "Not Registered? Create an account", if you don't have an account,Step 3: Fill out the form and click on sign up to create your account.
Step 4: Click on API on the menu

Step 5: Because we need the current weather data, we will need to subscribe to the Current Weather Data API subscription. It is the first option you will see in the menu. Click on Subscribe.Step 6: Now, the pricings window will open. We don't need any paid plan for this hobby project. So, select the free option here, and we are almost done.Step 7: After subscribing to it, in the top right corner, where your profile name appears, click on it, and select My API KeysStep 8: You will find your API key here. Keep it safe, and do not share it publicly with anyone.Now that we have our API key, we can move forward to building our app again.

In this app, we get the user's geolocation to show weather data according to the user's place. To get the geolocation data, we first have to know about the navigator object in JavaScript. The navigator object in JavaScript is used to fetch information related to the user agent or the browser. This object has a property called geolocation. By using this property, we can get the user's latitude and longitude. ----------------------------rest js part is basic you will easily get is if you know thw basic asynchronous javascript ainclude promises and navigator.geolocation
