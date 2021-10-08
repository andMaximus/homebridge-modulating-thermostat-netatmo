# homebridge-thermostat-netatmo

A netatmo thermostat plugin for homebridge, based on the new Netatmo energy API https://dev.netatmo.com/apidocumentation/energy
Initially this plugin will only allow for switching on and off the scheduled program. This will allow Homekit geofencing to turn of the scheduled heating program in case nobody is at home, which is currently not offered by the default Netatmo Homekit integration.

To use this plugin, you need to register an application on the Netatmo developer platform

1. Visit https://dev.netatmo.com/apps/createanapp#form (login with your netatmo account)
2. Fill out the required application fields
3. Copy and paste the client_id and client_secret into the configuration

# Configuration

```

"accessories": [
    {
        "accessory": "Netatmo Thermostat",
        "name": "Thermostat",
        "client_id": "<clientid from https://dev.netatmo.com/>",
        "client_secret": "<secret from https://dev.netatmo.com/>",
        "username": "",
        "password": ""
    }
],
