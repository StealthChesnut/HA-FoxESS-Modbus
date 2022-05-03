<h2 align="center">
   <a href="https://www.fox-ess.com">FoxESS</a> and<a href="https://www.home-assistant.io"> Home Assistant</a> integration via Modbus RS485
   </br></br>
   <img src="https://github.com/home-assistant/brands/raw/master/custom_integrations/foxess/logo.png" >
   </br>
</h2>


**A community maintained Home Assistant integration using local native polling of Modbus data using RS485 to enable near realtime data access, with no reliance on the FoxESS cloud portal**

---

⚠️**Requires additional hardware** ([RS485 to USB](https://www.amazon.co.uk/dp/B078X5H8H7?ref_=cm_sw_r_cp_ud_dp_CR8FQK7A50FNCH530QJP) or a [WIFI/LAN RS485](https://www.amazon.co.uk/dp/B07DNWM62H?ref_=cm_sw_r_cp_ud_dp_BPWX7Z53PDES4WJ9JY89) converter) & basic electronics competencies required to connect the two additional wires for the RS485 interface to the inverters com connector.⚠️

---


## Supported Hardware
**Hybrid Series** <br> <img align="right" src="https://user-images.githubusercontent.com/6324545/166170598-7077d481-4d65-49b5-9816-1873c97dd853.png" >
✅ H1-3.0-E <br>
✅ H1-3.7-E <br>
✅ H1-4.6-E <br>
✅ H1-5.0-E <br>
✅ H1-6.0-E <br>
**AC Series** <br>
✅ AC-3.0-E <br>
✅ AC-3.7-E <br>
✅ AC-4.6-E <br>
✅ AC-5.0-E <br>
✅ AC-6.0-E <br>

We strongly suspect that this plugin will also work with the FoxESS AIO series and 3PH series but have not yet tested. Please let us know if you have an AIO or 3PH system and if the plugin works.

---

<p>⚠️Warning: The structure and meaning of the data fields has been assumed, not drawn from official documentation. There may be errors - Use this at your own risk.</p>

The aim of this project is to enable the full use of the Energy dashboard in Home Assistant. The current status is most of this is functional, but there are a couple of todos:
* Find register and set up Utility Meter for Grid Consumption
* Find register and set up Utility Meter for Return to Grid

## Manual installation 
* Hardware configuration instructions can be found on the [wiki](https://github.com/StealthChesnut/HA-FoxESS-Modbus/wiki/)
* Take a copy / backup of your config and/or HA install before you change it! :)
* Copy the contents of the configuration.yaml file to your config file into the appropriate places
* Put the modbus.yaml file alongside your configuration.yaml file
* Check your config is valid, then Restart HA if so

## Engergy Dashboard Configuration

![image](https://user-images.githubusercontent.com/6324545/166470207-44236718-3f6c-4995-99fe-0a214eda49e6.png)
 

## Energy Dashboard Configuration

**Electricity Grid**

⚠️Some values won't appear until a small amount of data has passed through that value. You may need to wait 24hrs before you can setup the energy dashboard.

- grid_daily
- feedin_daily

**Solar Panels**

- pv1_daily
- pv2_daily

**Home Batteries**

- bat_charge_daily
- bat_discharge_daily

## Provided Entities

**Registers**

**The [wiki](https://github.com/StealthChesnut/HA-FoxESS-Modbus/wiki/Data-Register-Reference---H1-AC1) has references for the registers.**

<br>
<br>
Please read and understand before using this plugin:

> This plugin has been developed as a personal project, with no connection to the official brand of FoxESS, use of this plugin is intended for use by the community without fee but has no warrenty or liablity should any damage, harm or undesired results happen as a result of using this plugin. We strongly recommend that only competently trained individuals attempt to wire the additional connections required for this plugin to function. There is a risk of personal or device damage/harm.
You have been warned!

