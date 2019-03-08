# REST API: GET clicks (Marketing Suite)

Each emailing is tracked, which allows Copernica to provide you with 
emailing statistics. Clicks are one of these statistics. You can 
retrieve all clicks by sending an HTTP GET call to the following URL:

`https://api.copernica.com/v2/ms/clicks?access_token=xxxx`

This method also support the use of the [fields parameter](./rest-fields-parameter) 
for the **timestamp** field.

## Returned fields

The method returns a JSON object with several clicks. For each click 
the following information is available:

* **ID**: The ID of the click.  
* **mailing**: The ID of the mailing.
* **link**: The link that was clicked.
* **timestamp**: Timestamp of the click.
* **ip**: The IP where the click occurred from.
* **user-agent**: User agent string of the machine used to click.
* **destination**: The ID of the destination that clicked the link.
* **profile**: The ID of the profile that clicked the link.
* **subprofile**: The ID of the subprofile that clicked the link.

## PHP example

This script demonstrates how to use this API method:

```php
// dependencies
require_once('copernica_rest_api.php');

// change this into your access token
$api = new CopernicaRestAPI("your-access-token", 2);

// execute the call
print_r($api->get("ms/clicks"));
```

This example requires the [REST API class](./rest-php).

## More information

* [Overview of all REST API calls](./rest-api)
* [Get all abuses](./rest-get-ms-abuses)
* [Get all deliveries](./rest-get-ms-deliveries)
* [Get all errors](./rest-get-ms-errors)
* [Get all impressions](./rest-get-ms-impressions)