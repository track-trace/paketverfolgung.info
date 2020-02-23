<p align="center">
<a href="https://paketverfolgung.info"><img src="https://storage.googleapis.com/paketverfolgung-info/images/logos/paketverfolgung.info.gif" height="200"></a>
</p>

# paketverfolgung.info

A simple service to track parcels/shipments in multiple ways. It supports major shipping service provider like DHL, DPD, FedEx, GLS, Hermes, TNT, UPS and EMS - an international postal Express Mail Service, offered by postal operators of the Universal Postal Union (UPU) connecting more than 180 countries and territories worldwide.

The service paketverfolgung.info offers multiple ways to track your or the items of your customers. The clou is that you need only to enter valid tracking number of the supported shipping service provider. The service anaylise the tracking ID and redirect the user directly to the correct tracking page of the appropriate shipping service provider. With help of TrackLink&trade; and a browser integration, you or your customers do not even have to visit the site to get the tracking results. You also have the option of integrating the search field into your own page.


## Via webpage
<ol>
<li>Visit with a web browser https://paketverfolgung.info</li>
<li>Enter your tracking ID in the search form</li>
<li>hit enter or submit button</li>
</ol>

## Via TrackLink&trade; (aka WebHook)

TrackLink's replaces to original tracking link and are ideally to shorten and share via email, messenger, etc.

TrackLink consists of three segments:

**URL:** **`https://paketverfolgung.info`**`/ID/ {tracking_id}` <br>
**Identifier:** `https://paketverfolgung.info`**`/ID/`**`{tracking_id}` <br>
**Tracking ID:** `https://paketverfolgung.info /ID/`**`{tracking_id}`** <br><br>
In general the identifier is always **'ID'** as shown in the example below:<br>
Example: `https://paketverfolgung.info/ID/1Z9999999999999999`


## Via browser search (aka OpenSearch)

The browser integration of paketverfolgung.info allows you to use the browser address bar as a search input field, when needed, without visiting the original website before.

This function is called OpenSearch and works with Apple Safari, Microsoft Edge, Mozilla Firefox and Google Chrome. Before you can start using it, you have to setup your browser for this function. Here an example for Google Chrome:

At the top right, click More <img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/more.gif"> and then **Settings**.

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/google_chrome_settings.gif">

Under "Search engine," click **Manage search engines**.

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/manage_search_settings.gif">

To the right of "Other search engines," click **Add**.

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/search_engine_settings.gif">

Fill out the text fields as shown below and click **Add**.

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/edit_search_engine.gif" align="right">

**Search engine:**<br>
`Enter paketverfolgung.info or a name of your choice.`

**Keyword:**<br>
`Enter the character "p" or a keyword of your choice, to trigger later the search function.`

**URL with %s in place of query:**<br>
`https://paketverfolgung.info/OS/%s`

<br><br><br><br><br>

The setup is complete. You are still able to continue to enter a URL in the address bar or any search terms that trigger a Google search.

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/google_search_bar.gif">

The new feature is, if you enter an "p" followed by a space, then you activate the paketverfolgung.info search.

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/paketverfolgung.info_search_bar_1.gif">

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/paketverfolgung.info_search_bar_2.gif">

This cause that Google Chrome address bar react like the search field on this website. E.g. an UPS tracking ID, it will open UPS tracking result page.

<img src="https://storage.googleapis.com/paketverfolgung-info/images/browser_integration/chrome/paketverfolgung.info_search_bar_3.gif">

## Webpage integration

To integrate the search field into your own website a few line are needed. You can adjust the look and feel to your needs to keep your corporate identity:

```html
<form method="post" action="https://paketverfolgung.info/3P/">
  <input type="text" name="ID" placeholder="">
  <input type="submit" value="&#128269;">
</form>
```
