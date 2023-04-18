# Kora Pharmacy

SOS Pharma is a system designed to improve the exchange of pharmaceutical information on the availability of medicines between pharmacies and the consumers of their main service: the distribution of medicines.


**1. Drug stores SPA dashboard**
| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="500" height="250" alt="10" src="/img/linker/10.PNG">  |  <img width="500" height="250" alt="11" src="/img/linker/11.PNG">|<img width="500" height="250" alt="12" src="/img/linker/12.PNG">|

**2. Web application**
| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="500" height="250" alt="2" src="/img/doc/2.PNG"> |  <img width="500" height="250" alt="11" src="/img/doc/11.PNG">|<img width="500" height="250" alt="12" src="/img/doc/12.PNG">|

**3. Mobile application**
| | | | | |
|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="200" height="400" alt="4" src="/img/mobile/4.png">  |  <img width="200" height="400" alt="5" src="/img/mobile/5.png">|<img width="200" height="400" alt="8" src="/img/mobile/8.png">|  <img width="200" height="400" alt="11" src="/img/mobile/11.png">|<img width="200" height="400" alt="15" src="/img/mobile/15.png">|

**4. Drug stores SPA CMS (***incomplete***)**
| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="500" height="250" alt="1" src="/img/cms/1.PNG">  |  <img width="500" height="250" alt="2" src="/img/cms/2.PNG">|<img width="500" height="250" alt="3" src="/img/cms/3.PNG">|

## Description

 **1. Components**
 
The system consists of :
 - [ ] [<ins>Data</ins>](data) : a RestFull API to distribute information to the various other components and to collect their information.
 - [ ] [<ins>Linker</ins>](linker) : a single page application that interacts with the pharmacy's IS to collect information on medicines and share it with `data `
 - [ ] [<ins>Doc</ins>](doc) : an interactive web application providing an interface for users to view the informations of `data` (the API) from a web browser
 - [ ] [<ins>Mobile</ins>](mobile) : a mobile application allowing a mobile user to view the informations of `data` (the API) from their mobile device
 - [ ] [<ins>Id</ins>](id) : an authentication system interacting with firebase to secure access to `data` (the API) by `mobile` users
 - [ ] [<ins>CMS ***(incomplete)***</ins>](cms) : a single page application for drug store administration. The application provide an interface to help pharmacists manage their information systems
 
 **2. Conception**

 - [ ] [<ins>Data</ins>](data) : native PHP application built with a custom library developped by us based on MVC pattern
 - [ ] [<ins>Linker</ins>](linker) : made with HTML, Javascript with custom personnal framework to build a single page application, CSS3, Twig, PHP built with a custom personnal library developped by us based on MVC pattern
 - [ ] [<ins>Doc</ins>](doc) : buuit with HTML, Javascript, CSS3, Twig, PHP built with a custom personnal library developped by us based on MVC pattern
 - [ ] [<ins>Mobile</ins>](mobile) : built with Dart and Flutter with a custom library based on dart
 - [ ] [<ins>Id</ins>](id) : built with PHP
 - [ ] [<ins>CMS ***(incomplete)***</ins>](cms) : made with HTML, Javascript with custom personnal framework to build a single page application, CSS3, Twig, PHP built with a custom personnal library developped by us based on MVC pattern

All these components are based on a native personnal library (PHP, Javascript).

## Get started
 
 **1. <ins>Install database</ins>**
 
 Use the sql files on [<ins>db</ins>](db) directory to create the database.
 
 **2. <ins>Setup `data`</ins>**
 
 Setup [<ins>data</ins>](data) and set database config and http links in [<ins>config file</ins>](data/config.php).
 
 **3. <ins>Setup `id`</ins>**
 
 Setup [<ins>id</ins>](id) and set database config and http links in [<ins>config file</ins>](data/config.php).
 
 **4. <ins>Setup `linker`</ins>**
 
 Deploy [<ins>linker</ins>](linker) then launch setup assistant to configure the dashboard.
 
 Follow instruction in [<ins>readme file</ins>](linker/README.md#get-started)
 
 **5. <ins>Deploy `doc`</ins>**
 
 Setup [<ins>doc</ins>](doc) and set http links in [<ins>config file</ins>](data/config.php) to connect it with [<ins>data</ins>](data).
 
 **6. <ins>Deploy `mobile`</ins>**
 
 Setup [<ins>mobile</ins>](mobile) and set http links in [<ins>config file</ins>](mobile/lib/datas/request/endpoint.dart) to connect it with [<ins>data</ins>](data).
 
 **7. <ins>`cms`</ins>(***incomplete***)**
 
Setup [<ins>cms</ins>](cms) and set database config and http links in [<ins>config file</ins>](cms/config.php). 

This module does not work with previous ones. It is completely isoleted from others.
