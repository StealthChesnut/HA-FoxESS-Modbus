## ⚠️ Not yet stable, modbus & config file under regular change until v1.0 due Friday 6th May ⚠️

<h2 align="center">
   <a href="https://www.fox-ess.com">FoxESS</a> and<a href="https://www.home-assistant.io"> Home Assistant</a> integration via Modbus RS485
   </br></br>
   <img src="https://github.com/home-assistant/brands/raw/master/custom_integrations/foxess/logo.png" >
   </br>
</h2>


**A community maintained Home Assistant integration using local native polling of Modbus data using RS485 to enable near realtime data access, with no reliance on the FoxESS cloud portal**

![image](https://user-images.githubusercontent.com/6324545/166502285-eb0ca405-05a3-4722-a698-36e3e6b0f60d.png)


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

<p>The aim of this project is to enable the full use of the Energy dashboard in Home Assistant and is a fully functional replacement of the FoxESS App for reporting needs.</p>

## Manual installation
* Hardware configuration instructions can be found on the [wiki](https://github.com/StealthChesnut/HA-FoxESS-Modbus/wiki/)
* Create a full backup of your HA instance including the configuration.yaml file
* Copy the contents of the [configuration.yaml](https://github.com/StealthChesnut/HA-FoxESS-Modbus/blob/main/configuration.yaml) file to your config file
* Create a new file called [modbus.yaml](https://github.com/StealthChesnut/HA-FoxESS-Modbus/blob/main/modbus.yaml) and place alongside your configuration.yaml file
* Check your config is valid, then Restart HA
* Map energy dashboard as per below example and enjoy configuring dashboards using near realtime data.


[Step by step walkthrough of the setup](https://youtu.be/uMPr0V6lTHg)
![image](https://user-images.githubusercontent.com/6324545/166504169-81fd77e8-df5b-40f0-9c1f-9735e59b2723.png)

## Engergy Dashboard Configuration

![image](https://user-images.githubusercontent.com/6324545/166470207-44236718-3f6c-4995-99fe-0a214eda49e6.png)
 

### Energy Dashboard Values

⚠️Some values won't appear until a small amount of data has passed through that value. You may need to wait 24hrs before you can setup the energy dashboard.

**Electricity Grid**
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

