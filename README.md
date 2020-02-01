# thermostat-server
Raspberry Pi based Boiler Control unit

This unit will be used to control a set of relays will apply power to zone control valves.
This will be used in place of more traditional HVAC thermostats.
Each zone will have a Raspberry Pi that will be queried by the server to get the current temperature.
Each Raspberry Pi client will have a connected 1-wire DS18B20 to provide the current reading.
Each Raspberry Pi will also use PoE.



The server will have NAT and DHCP installed. The NIC will be used to communicate with the thermostat clients.
The Wifi interface will be used to connect to the outside word.

Information dealing with heating will reside in SQLite.


There will also be pulling of information from the National Weather Service
https://www.weather.gov/documentation/services-web-api

More information will follow.

Installation Notes.

Installation Script:
sudo apt install sqlite
