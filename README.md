# Using the OnPoint API with Postman

[OnPoint® Weather](https://weathersource.com/products/onpoint-weather/) is available on demand via the [OnPoint API](https://developer.weathersource.com/) ensuring immediate access to hyper-local global analytics grade weather data.

[Postman](https://www.getpostman.com/) is a powerful GUI platform for faster and easier API development.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/ce7a3abf5ca6e28ff776)


## Installing the OnPoint API Collection

Download and install a copy of Postman from [getpostman.com/apps](https://www.getpostman.com/apps).

Once installed, click the [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/ce7a3abf5ca6e28ff776) button.

Select the installed Postman application (Postman for Chrome or Postman for Mac/Windows/Linux) from the prompt.

![Open with...](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/open-with.png?raw=true)

Postman will open and import the OnPoint API collection.

![Collection Installed](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/collection-installed.png?raw=true)


## Configure an Environment

To use the OnPoint API collection in Postman, you need an OnPoint API Key. Get a free 30-day Developer Key at the [Weather Source Developer Portal](https://developer.weathersource.com/#developer-account-sign-up).

Once you have an OnPoint API Key, store it in a Postman environment variable named `onpoint_key`. Follow Postman's documentation to [set up an environment with variables](https://www.getpostman.com/docs/postman/environments_and_globals/manage_environments). The screenshot below shows a Postman environment configured with the `onpoint_key` variable.

![Configured Environment](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/configured-environment.png?raw=true)


## Free Developer Access Levels

The free 30-day Developer Key grants access to the following requests:

* History Postal Code
* Forecast Postal Code
* Nowcast Postal Code
* Astronomy Postal Code
* Postal Code Metadata

If you need access to other resources, increased throughput allowance, or a license for production use, please email <sales@weathersource.com> or call (844) 813-2617.


## Using the OnPoint API Collection

View full documentation for the OnPoint API at the [Weather Source Developer Portal](https://developer.weathersource.com/documentation/).

The OnPoint API collection groups request types in the following folders:

* History
* Forecast
* Nowcast
* Climatology
* Astronomy
* Location Metadata

Each request type may query by Latitude/Longitude, Postal Code, Nielsen Designated Marketing Area, or OnPoint ID. History, Forecast, Nowcast, and Climatology also have geospatial data in GeoJSON, SHP, GeoTIFF, and PNG formats.

Open a folder and select a request. This screenshot shows the History Postal Code request.

![History Postal Code](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/history-postal-code.png?raw=true)

Page description (yellow) and parameter descriptions (green) provide limited documentation for the selected request. Detailed resource documentation is available at the [Weather Source Developer Portal](https://developer.weathersource.com/documentation/resources/).

The request URL (red) contains variables (in addition to `onpoint_key`). In this example, `postal_code`, `country`, and `format` should be replaced with values of your choosing. By default, values are set to `22222`, `us`, and `json` respectively.

Submit the request.
