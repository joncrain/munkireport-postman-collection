# MunkiReport Postman Collection

## Overview

This collection is provided to assist MunkiReport users of the API. It provides a quick method to interact with most endpoints.

This article describes the recommended Postman configuration and setup process to import the collection, configure variables to connect it to your MunkiReport environment and begin testing API calls and interacting with your MunkiReport environment via the API

## Import the Collection

Use the following options to import the collection into Postman:

* Click the [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/c45e1e3efc209186c272) button to automatically import the collection into your Postman app.
* In Postman, click File >> Import.
  * Download the JSON included in this repo and select the .json file.

## Define Environment Variables

This collection utilizes the following variables which should be defined within one of the scopes in Postman. The example variables are defined within the collection. (Go to the Variable tab under edit collection)

| Variable          | Description                                        | Example           |
|-------------------|----------------------------------------------------|-------------------|
| {{mr-url}}        | Hostname and port of the MunkiReport environment   | munki.example.com |
| {{mr-login}}      | Username to authenticate to MunkiReport with       | administrator     |
| {{mr-password}}   | Password of the user authenticating to MunkiReport | pa$$word          |
| {{serial_number}} | Example of serial number to call                   | C02000QWFVH6      |

## Getting Started

After the collection has been imported and valid values have been defined for the variables, the Authentication request should be called to create a cookie for the MunkiReport instance. Additional requests should be able to use this session.

## Troubleshooting

You may need to disable the SSL certificate verification to talk to the MunkiReport server. Or that could just be a weird issue with my certs.