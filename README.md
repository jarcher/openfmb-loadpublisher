# README #

Refer to [Wiki](https://github.com/openfmb/dtech-demo-2016/wiki) for information on DTech Demo

# Description
The loadpubliser is a java application that publishes the OpenFMB Phase I Resource Reading using MQTT.

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

Loadpublisher is available under the Apache 2.0 license. See the APACHE_FILE_HEADER file for more info.
