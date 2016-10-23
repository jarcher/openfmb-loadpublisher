![Logo of the Project](https://github.com/openfmb/dtech-demo-2016/blob/master/img/openfmb-tm-black_reduced_100.png)

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

## Contributing

David Lawrence, Duke Energy,  <email>

Dwayne Bradley, Duke Energy, <email>

If you'd like to contribute, please fork the repository and use a feature
branch. Pull requests are warmly welcome.

# License

See the [APACHE_FILE_HEADER](https://github.com/openfmb/openfmb-common-mqtt/blob/master/APACHE_FILE_HEADER) file for more info.
___________________________________________________

# Name of the project
> Additional information or tagline

A brief description of your project, what it is used for and how does life get
awesome when someone starts to use it.

## Installing / Getting started

A quick introduction of the minimal setup you need to get a hello world up &
running.

```shell
packagemanager install awesome-project
awesome-project start
awesome-project "Do something!"  # prints "Nah."
```

Here you should say what actually happens when you execute the code above.

## Developing

Here's a brief intro about what a developer must do in order to start developing
the project further:

```shell
git clone https://github.com/your/awesome-project.git
cd awesome-project/
packagemanager install
```

And state what happens step-by-step.

### Building

If your project needs some additional steps for the developer to build the
project after some code changes, state them here:

```shell
./configure
make
make install
```

Here again you should state what actually happens when the code above gets
executed.

### Deploying / Publishing

In case there's some step you have to take that publishes this project to a
server, this is the right time to state it.

```shell
packagemanager deploy awesome-project -s server.com -u username -p password
```

And again you'd need to tell what the previous code actually does.

## Features

What's all the bells and whistles this project can perform?
* What's the main functionality
* You can also do another thing
* If you get really randy, you can even do this

## Configuration

Here you should write what are all of the configurations a user can enter when
using the project.

#### Argument 1
Type: `String`  
Default: `'default value'`

State what an argument does and how you can use it. If needed, you can provide
an example below.

Example:
```bash
awesome-project "Some other value"  # Prints "You're nailing this readme!"
```

#### Argument 2
Type: `Number|Boolean`  
Default: 100

Copy-paste as many of these as you need.


When you publish something open source, one of the greatest motivations is that
anyone can just jump in and start contributing to your project.

These paragraphs are meant to welcome those kind souls to feel that they are
needed. You should state something like:
