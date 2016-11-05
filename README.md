![Logo of the Project](https://github.com/openfmb/dtech-demo-2016/blob/master/img/openfmb-tm-black_reduced_100.png)

# Description
The loadpubliser is a java application that publishes the OpenFMB Phase I Resource Reading Profile using MQTT and uses the [openfmb_common_mqtt repo](https://github.com/openfmb/openfmb-common-mqtt).  The loadpublisher is designed to be part of the overall Dtech Demo.  It uses the kW load Table in the properties file to pusblish values (kW).  The load table is composed of 24 hourly values and the publisher interpolates between the values with adds jitter to be published at the MQTT publish rate parameter.

# Installing / Getting started

A quick introduction of the minimal setup you need to get the loadpublisher up & running.  NOTE: This project is used in the Dtech Demo.  Refer to [Wiki](https://github.com/openfmb/dtech-demo-2016/wiki) for information on DTech Demo.  You can separately install and run the project but you will need to additionaly install a MQTT broker and other processes depending on your use.  Also dependencies such as JAVA, GIT and the MQTT Broker are described in the Wiki above

```shell
java -cp openfmb-loadpublisher-1.0-jar-with-dependencies.jar com.dukeenergy.eto.openfmb.LoadPublisher
```
The loadpublisher jar above can we run with the entry point provided.  

## Dependencies

Please refer to the Wiki pages for the [Demonstration]https://github.com/openfmb/turnkey-dtech-demo-2016/wiki/Simulation-Demonstration] and (Prerequisites)[https://github.com/openfmb/turnkey-dtech-demo-2016/wiki/Simulation-Prerequisites].


## Building

The loadpublisher is dependent on the [openfmb-common-mqtt](https://github.com/openfmb/openfmb-common-mqtt) repository.  To build the loadpublisher do the following:

```shell
git clone https://github.com/openfmb/openfmb-loadpublisher.git
cd openfmb-loadpublisher
mvn clean install
```
The build jar is put in the target directory and needs to be moved to the main directory where the properities files are located. 


## Configuration
The main configuration file is called "[LoadPublisher.properties](https://github.com/openfmb/openfmb-loadpublisher/blob/master/loadpublisher/LoadPublisher.properties)".  The user can set a number of parameters to affect the behavior of the application including the following:
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

# Contributing

David Lawrence, Duke Energy,  <email>

Dwayne Bradley, Duke Energy, <email>

If you'd like to contribute, please fork the repository and use a feature
branch. Pull requests are warmly welcome.

Please review the [CONTRIBUTING](https://github.com/openfmb/openfmb-simulators/blob/master/CONTRIBUTING.md) file. 

# License

See the [APACHE_FILE_HEADER](https://github.com/openfmb/openfmb-loadpublisher/blob/master/APACHE_FILE_HEADER) file for more info.
