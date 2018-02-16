# Using the OnPoint API with Postman

The [OnPoint® API](https://developer.weathersource.com/) by [Weather Source](https://weathersource.com/) provides hyper-local past, present & forecast weather data for business intelligence on a global scale.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/ce7a3abf5ca6e28ff776)


## Installing the OnPoint API Collection

If the Postman application is not installed, download and install a copy from Postman's [Native Applications](https://www.getpostman.com/apps) page.

Once Postman is installed, click the [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/ce7a3abf5ca6e28ff776) button.

Postman will prompt a selection of a Postman application (Postman for Chrome or Postman for Mac/Windows/Linux) to import the OnPoint API collection. Select the installed application.

![Open with...](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/open-with.png?raw=true)

Once you make a selection, the Postman application will open and import the OnPoint API collection.

![Collection Installed](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/collection-installed.png?raw=true)


## Configure an Environment

To use the OnPoint API collection in Postman, you need an OnPoint API Key. Get a free 30-day Developer Key at the [Weather Source Developer Portal](https://developer.weathersource.com/#developer-account-sign-up).

Once you have an OnPoint API Key, it store it in a Postman environment variable named `onpoint_key`. Follow Postman's documentation to [set up an environment with variables](https://www.getpostman.com/docs/postman/environments_and_globals/manage_environments). The screenshot below shows a Postman environment configured with the `onpoint_key` variable.

![Configured Environment](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/configured-environment.png?raw=true)


## Free Developer Access Levels

The free 30-day Developer Key grants access to the following requests:

* History Postal Code
* Forecast Postal Code
* Nowcast Postal Code
* Astronomy Postal Code
* Postal Code Metadata

If you need access to the other resources, higher throughput allowance, or license to use the API in a production environment, please email <sales@weathersource.com> or call (844) 813-2617.


## Using the OnPoint API Collection

View full documentation for the OnPoint API at the [Weather Source Developer Portal](https://developer.weathersource.com/documentation/).

The OnPoint API collection groups request types in the following folders:

* History
* Forecast
* Nowcast
* Climatology
* Astronomy
* Location Metadata

Each request type may query by Latitude/Longitude, Postal Code, Nielsen Designated Marketing Areas, or OnPoint IDs. History, Forecast, Nowcast, and Climatology also have geospatial data in GeoJSON, SHP, GeoTIFF, and PNG formats.

Open a folder and select a request. This screenshot shows the History Postal Code request.

![History Postal Code](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/history-postal-code.png?raw=true)

Each request is documented in the page description (yellow) and parameter descriptions (green). More detailed documentation for each resource is available at the [Weather Source Developer Portal](https://developer.weathersource.com/documentation/resources/).

The request URL (red) contains variables (in addition to `onpoint_key`). In this example, `{{postal_code}}`, `{{country}}`, and `{{format}}` should be replaced with the values of your choosing. By default, values are set to `22222`, `us`, and `json` respectively.

Press "Send" to submit the request, and data will be returned in the requested format.
