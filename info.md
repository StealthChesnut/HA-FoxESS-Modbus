# HA-FoxESS-Modbus
Home Assistant Modbus Integration setup for Fox ESS H1 Inverter

Warning: The structure and meaning of the data fields have been guessed, not drawn from official documentation. There may be errors - Use this at your own risk.

The aim of this project is to enable the full use of the Energy dashboard in Home Assistant. The current status is most of this is functional, but there are a couple of todos:
* Find register and set up Utility Meter for Grid Consumption
* Find register and set up Utility Meter for Return to Grid

Steps:
* Take a copy / backup of your config and/or HA install before you change it! :)
* Copy the contents of the configuration.yaml file to your config file into the appropriate places
* Put the modbus.yaml file alongside your configuration.yaml file
* Check your config is valid, then Restart HA if so

Energy Dashboard Config:

*Electricity Grid*

--in progress--

*Solar Panels*

Select the solar_production__um_daily sensors

*Home Batteries*

Select the Battery Dis/Charge Rate sensors





The Wiki has a reference for the registers.

