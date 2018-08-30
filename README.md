<p align="center">
  <img alt="logo" src="https://raw.githubusercontent.com/AresS31/swurg/master/images/logo2.png" height="200">
  <p align="center">
      <a href="https://portswigger.net/bappstore/6bf7574b632847faaaa4eb5e42f1757c"><img alt="bapp store" src="https://img.shields.io/badge/BApp-Published-orange.svg"></a>
      <a href="https://www.java.com"><img alt="lang" src="https://img.shields.io/badge/Lang-Java-blue.svg"></a>
      <a href="https://opensource.org/licenses/Apache-2.0"><img alt="license" src="https://img.shields.io/badge/License-Apache%202.0-red.svg"></a>
      <img alt="version" src="https://img.shields.io/badge/Version-2.2-green.svg">
      <img alt="bitcoin" src="https://img.shields.io/badge/Bitcoin-15aFaQaW9cxa4tRocax349JJ7RKyj7YV1p-yellow.svg">
      <img alt="bitcoin cash" src="https://img.shields.io/badge/Bitcoin%20Cash-qqez5ed5wjpwq9znyuhd2hdg86nquqpjcgkm3t8mg3-yellow.svg">
      <img alt="ether" src="https://img.shields.io/badge/Ether-0x70bC178EC44500C17B554E62BC31EA2B6251f64B-yellow.svg">
  </p>
</p>

## Swurg is a Burp Suite extension for RESTful API testing.
During penetration testing of RESTful APIs, it can be time consuming to chain the Burp Suite with other tools such as `SOAP-UI`. However, this is often necessary to parse the desriptions provided by APIs for use with the Burp Suite scanning capabilities. 

**Swurg** is a RESTful API parser allowing security professionals to use the Burp Suite as the only tool for testing RESTful APIs engagements. The following screenshot shows the plugin interface:

<img alt="ui" src="https://raw.githubusercontent.com/AresS31/swurg/master/images/ui.png" width="400" />

## Supported Features
* Parse OpenAPI specifications, previously known as Swagger specifications, supporting JSON and YAML formats.
* Parse OpenAPI specifications from URLs and files - *they can directly be sent to the extension from the site map using the 'Send to Swagger Parser' option in the context menu*.
* Send requests to the Intruder, Reapeater, Scanner and Site map.
* Responsive GUI.

## Installation
### Compilation 
#### Windows & Linux
1. Install gradle (<https://gradle.org/>)
2. Download the repository.
```console
$ git clone https://github.com/AresS31/swurg
$ cd .\swurg\
```
3. Create the swurg jarfile:
```console
$ gradle fatJar
```

### Burp Suite settings
In the Burp Suite, under the `Extender/Options` tab, click on the `Add` button and load the `swurg-all` jarfile. 

## Possible Improvements
- [ ] Add new features
- [ ] Source code optimisation

## Dependencies
### Third-party libraries
#### Swagger Parser:
The *Swagger Parser* library is required and imported in this project. 

<https://mvnrepository.com/artifact/io.swagger/swagger-parser/1.0.33>

## Project information
In July 2016, after posting a request for improvement on the [PortSwigger support forum](https://support.portswigger.net/customer/portal/questions/16358278-swagger-parser-and-wsdler-improvement), I decided to take the lead and implement a solution myself.

The extension is still in development, feedback and comments are much appreciated.

## Donation
If you want to support my work doing a donation, it will be very much appreciated:
* Bitcoin       : **15aFaQaW9cxa4tRocax349JJ7RKyj7YV1p**
* Bitcoin Cash  : **qqez5ed5wjpwq9znyuhd2hdg86nquqpjcgkm3t8mg3**
* Ether         : **0x70bC178EC44500C17B554E62BC31EA2B6251f64B**

## License
Copyright (C) 2016 - 2018 Alexandre Teyar

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
