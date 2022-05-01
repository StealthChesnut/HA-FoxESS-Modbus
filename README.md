<h2 align="center">
   <a href="https://www.fox-ess.com">FoxESS</a> and<a href="https://www.home-assistant.io"> Home Assistant</a> integration via Modbus RS485
   </br></br>
   <img src="https://github.com/home-assistant/brands/raw/master/custom_integrations/foxess/logo.png" >
   </br>
</h2>


<b>A community maintained Home Assistant integration using local native polling of data using RS485 over Modbus to enable near realtime data access, with no reliance on the FoxESS cloud portal</b><br><br>
Home Assistant Modbus Integration setup for Fox ESS H1 Series Inverters

---

⚠️Requires additional hardware (RS485 to USB or a WIFI/LAN RS485 converter) and basic electronics competencies required to connect the two additional wires for the RS485 interface to the inverters com connector.⚠️
---

<p>Warning: The structure and meaning of the data fields have been guessed, not drawn from official documentation. There may be errors - Use this at your own risk.</p>

The aim of this project is to enable the full use of the Energy dashboard in Home Assistant. The current status is most of this is functional, but there are a couple of todos:
* Find register and set up Utility Meter for Grid Consumption
* Find register and set up Utility Meter for Return to Grid

Steps:
* Take a copy / backup of your config and/or HA install before you change it! :)
* Copy the contents of the configuration.yaml file to your config file into the appropriate places
* Put the modbus.yaml file alongside your configuration.yaml file
* Check your config is valid, then Restart HA if so


## Energy Dashboard Configuration

*Electricity Grid*

--Coming Soon--

**Solar Panels**

 ## Select the solar_production__um_daily sensors 

**Home Batteries**

 # Select the Battery Dis/Charge Rate sensors

---

**The [wiki](https://github.com/StealthChesnut/HA-FoxESS-Modbus/wiki/Data-Register-Reference---H1-AC1) has references for the registers.**


