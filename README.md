# Using the OnPoint® API with Postman

The [OnPoint API](https://developer.weathersource.com/) by [Weather Source](https://weathersource.com/) provides hyper-local past, present & forecast weather data for business intelligence at a global scale.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/ce7a3abf5ca6e28ff776)

## Installing the OnPoint API Collection

If you do not already have the Postman app installed, download and intall a copy from Postman's [Native Apps](https://www.getpostman.com/apps) page.

Once Postman is installed, click the [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/ce7a3abf5ca6e28ff776) button.

Postman will propmt a selection of Postman applications (Postman for Chrome or Postman for your native OS) with which to open the OnPoint API collection. Select the application you have installed.

![Open with...](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/open-with.png?raw=true)

Once you have made a selection, the Postman application will be opened and the collection will be imported.

![Collection Installed](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/collection-installed.png?raw=true)

## Configuring an Environment

To use the OnPoint API collection in Postman, you will need an OnPoint API Key. Get a free 30-day Developer Key at the [Weather Source Developer Portal](https://developer.weathersource.com/#developer-account-sign-up).

Once you have a OnPoint API Key, it should be stored to a Postman environment variable named `onpoint_key`. Follow Postman's documentation to [set up an environment with variables](https://www.getpostman.com/docs/postman/environments_and_globals/manage_environments). The screenshot below shows a Postman environment configured with the `onpoint_key` variable.

![Configured Environment](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/configured-environment.png?raw=true)

## Free Developer Access Levels

The free 30-day Developer Key will give you access to the following requests:

* History Postal Code
* Forecast Postal Code
* Nowcast Postal Code
* Astronomy Postal Code
* Astronomy Postal Code
* Postal Code Metadata

If you need access to the other resources, higher throughput allowance, or license to use the API in a production environment, please email <sales@weathersource.com> or call (844) 813-2617.

## Using the OnPoint API Collection

Full documentation for the OnPoint API can be found at the [Weather Source Developer Portal](https://developer.weathersource.com/documentation/).

The OnPoint API collection has requests broken down into the following folders:

* History
* Forecast
* Nowcast
* Climatology
* Astronomy
* Location Metadata

Each folder has access to data by Latitude/Longitude, Postal Code, Nielsen Designated Marketing Areas, and OnPoint IDs. The first four folders also have access to geospatial data in GeoJSON, SHP, GeoTIFF, and PNG formats.

Open a folder and select a request. Here we have selected the History Postal Code request.

![History Postal Code](https://github.com/weathersource/postman-collection-onpoint-api/blob/master/assets/history-postal-code.png?raw=true)

Each request has been documented in the page description (yellow) and parameter descriptions (green). More detailed documentation is available for each resource at the [Weather Source Developer Portal](https://developer.weathersource.com/documentation/resources/).

The request URL (red) has vairables that are populated with sample data. In this example, `{{postal_code}}`, `{{country}}`, and `{{format}}` are prepopulated with the values of `22222`, `us`, and `json` respectively. These variables can be replaced with the values of your choosing.

Press "Send" to submit the request, and data will be returned in the requested format.
