# solcast
Used to downloa dand display the solar forecast from Solcast

This code downloads a solar forecast for use with home automation within node-red.

Firstly you need to setup an account with solcast.
https://solcast.com/

Setup your site with details on your solar panels, size, orientation etc.  This will then provide you with a site ID an authentication details.

You will need to edit the http node (SolarForecast) in node-red.  Change the URL to include your resource-id and also change the bearer token.

Resource ID is the API URL from the solcast site page
Bearer tolken is the API key which comes from your account page in solcast.

By default it’s scheduled to run every hour.

DEPENDANCIES

node-red-contrib-moment – This is used on the dash to provide a nice human statement about when the last URL update was.  You can remove this without impacting anything.
