# README #
![Logo of the Project](https://github.com/openfmb/dtech-demo-2016/blob/master/img/Open%20FMB%20Logos.png)
Refer to [Wiki](https://github.com/openfmb/dtech-demo-2016/wiki) for information on DTech Demo

# Description
The loadpubliser is a java application that publishes the OpenFMB Phase I Resource Reading Profile using MQTT and uses the [openfmb_common_mqtt repo](https://github.com/openfmb/openfmb-common-mqtt).  The loadpublisher is designed to be part of the overall Dtech Demo.  It uses the kW load Table in the properties file to pusblish values (kW).  The load table is composed of 24 hourly values and the publisher interpolates between the values with adds jitter to be published at the MQTT publish rate parameter.


# Configuration
The main configures file is called "[LoadPublisher.properties](https://github.com/openfmb/openfmb-loadpublisher/blob/master/loadpublisher/LoadPublisher.properties)".  The user can set a number of parameters to including the following:
+ MQTT Broker IP and Host
+ SSL Configuration Information
+ MQTT QOS
+ MQTT Publish Rate
+ kW Load Table
+ OpenFMB
  + Logical Device ID
  + MRID 
  + Desc
  + Name

# Author(s)

David Lawrence, Duke Energy,  <email>

Dwayne Bradley, Duke Energy, <email>


# License

See the [APACHE_FILE_HEADER](https://github.com/openfmb/openfmb-common-mqtt/blob/master/APACHE_FILE_HEADER) file for more info.
