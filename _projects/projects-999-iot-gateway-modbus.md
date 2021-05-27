---
title: "Google IoT Gateway for Modbus"
excerpt: "A MQTT Gateway connecting Modbus RTU and Google IoT Core <br/><img src='../images/projects/logo_iot_gateway_modbus.svg' height='300' width='500' alt='Modbus Raspberry Google IoT Core'>"
collection: projects
---

# IoT_Gateway_Modbus: 
# A MQTT Gateway connecting Modbus RTU with MQTT Bridge of Google IoT Core

This software is a user-solution of an "IoT Gateway" for Modbus RTU. 

The intitial reason for starting this solution was the need for a Gateway for Solar Microgrids.
A monitoring system for microgrids can help NGOs and companies e.g. in Eastern Africa, to prove project success and also improves predictive and reliable maintainance. 
Using a small embedded Linux/Windows computer, e.g. a Raspberry PI, low-cost Modbus RTU sensors can be read and a cost-effective monitoring solution is possible. 

## As provided this solution offers:
- Cloud: Google IoT Core
	- deploying and changing Modbus configuration from the GCP.
	- Reliable connection using Python Paho MQTT Client
	- low data footprint in GSM szenarios: compression of multiple sensor measurements using gzip  

- Modbus: Modbus RTU: RS232, RS485 via USB interface.
	- read sensor values from 5-10 Modbus RTU Slaves per second
	- schedule individual indivdual for each sensor and slave

You can find out more about this project in [my github repo](https://github.com/michaelfeil/iot_gateway_modbus).

![image info]({{ site.baseurl }}{% link images/projects/overview_iot_gateway_modbus.svg %}) 
This code example works with google IoT Core and other MQTT Briges. However, this code it not affiated with products of Google or Google Cloud.