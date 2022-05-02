# IH2

"Intelligent house 2" is an extension of The Intelligent House. Links to the previous project:

 - [Gitlab repo](https://gitlab.com/InuitViking/the-intelligent-house)
 - [Library repo](https://gitlab.com/InuitViking/libtih)

Just like the previous project, this will be hosted on [Gitlab](https://gitlab.com/InuitViking/ih2), but I will make sure to mirror it to [Github](https://github.com/inuitviking/IH2).

This project will be split into various projects, as to not confuse the programmer.
Proper documentation will appear in *this* repository, and links to the other projects will appear below.

## Table of Contents
[[_TOC_]]

*Note:* If the table of contents is missing, [go to the Gitlab repository instead](https://gitlab.com/InuitViking/ih2).

## Wiki
General in-depth documentation can be found [here](https://gitlab.com/InuitViking/ih2/-/wikis/home).

## List of repositories

- [IH2 (documentation - this repository)](https://gitlab.com/InuitViking/ih2)
- [IH2 for MKR1010](https://gitlab.com/InuitViking/ih2_mkr1010)

## Requirements

### School requirements
 - [ ] To read values from sensors wirelessly, and process that data with the intention to make statistics, which can be used to optimise resource usage and health.
 - [ ] To remotely control e.g. temperature and ventilation via a web interface.
 - [ ] To prepare the readings to be presented in a mobile app.
 - [ ] To make it so that relevant devices communicate with each other, either by wireless or wired protocols.
 - [ ] To make a good documentation, which gives programmers fast information to use for debugging and configuration.

### Personal requirements
 - [x] Make use of MKR Wifi 1010 to upload sensor reading via MQTT.
    - [x] From self
    - [ ] If there's time, also from other boards.
 - [ ] Make use of other devices and MQTT services to send commands to the board(s) via MQTT.
    - [ ] Via MQTT clients
    - [ ] If there's time, a custom (quickly made) web interface and/or CLI.
 - [ ] Make use of MKR WiFi 1010 to authenticate cards.
    - [ ] Via a local array.
    - [ ] If there's time, also with an online database via HTTP requests; could also be a local raspberry pi.
 - [ ] Make use of a knob to have a menu after login.
 - [ ] Make use of the RTC.

#### If there is time, these are also some extensions to the above requirements.
 - [ ] Make use of a database and an online API for the MKR WiFi 1010 to communicate with (both MQTT and HTTP).
    - [ ] MariaDB to store authorised cards.
    - [ ] Web server to handle the POST and GET requests
 - [ ] Send warnings and errors to an online API.
    - [ ] Discord API (create a bot or websocket); This one is the easiest, so this one first.
    - [ ] Self Made API.
 - [ ] Sync RTC via the internet.

#### Components
 - [x] MKR WiFi 1010 (Board)
 - [ ] RFID-RC522 (RFID Reader)
 - [ ] DS3231 (Real Time Clock)
 - [x] SSD1306 (OLED Display)
 - [x] DH11 (Temperature And Humidity Reader)
 - [ ] MicroServo 9G SG90 (Servo Motor)
 - [ ] LEDs

##### If there is time, also include these:
 - [ ] L293D - For communicating with a generic DC motor.
 - [ ] ELEGOO Power MB V2
 - [ ] 28BYJ-48 Stepper Motor
 - [ ] 4 Phase ULN2003 Stepper Motor Driver PCB

### Requirement notices
I may or may not be able to use all of these, but focus will be on the wireless parts, such as the following:
- Communicating with a remote service
    - To send sensor data to (MQTT)
    - To read commands from (MQTT)
    - To send requests to (HTTP)
    - To read general data from (HTTP)
- Controlling components
    - Locally via a menu
    - Remotely via an interface

The rest will come if there is time for it, such as potentially connecting a secondary board.

## Software, Libraries, Languages, and Services
### Software
 - Clion
 - Platform.io
 - PopOS 22.04
 - AVRDude

#### Potentially if there is time
 - Debian 11
 - MariaDB
 - Apache / NGINX
 - Mosquitto

### Languages
 - C++ (Arduino specific)
 - BASH

#### Potentially if there is time
 - PHP
 - MariaDB flavoured SQL
 - JavaScript (not too sure about this, though).

### Libraries
#### C++
 - Arduino.h

### Services
 - ThingSpeak / Shiftr.io (whatever I find more useful)

#### Potentially if there is time
 - Discord API
 - Self-made API
 - Self-hosted Mosquitto (open source MQTT broker)
