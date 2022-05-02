# IH2

"Intelligent house 2" is an extension of The Intelligent House.

 - [Gitlab repo](https://gitlab.com/InuitViking/the-intelligent-house)
 - [Library repo](https://gitlab.com/InuitViking/libtih)

Just like the previous project, this will be hosted on Gitlab, but I will make sure to mirror it to Github.

This project will be split into various projects, as to not confuse the programmer.
Proper documentation will appear in *this* repository, and links to the other projects will appear below.

## Table of Contents
[[_TOC_]]

## List of repositories

- [IH2 (documentation - this repository)](https://gitlab.com/InuitViking/ih2)

## Requirements

### School requirements
 - [ ] To read values from sensors wirelessly, and process that data with the intention to make statistics, which can be used to optimise resource usage and health.
 - [ ] To remotely control e.g. temperature and ventilation via a web interface.
 - [ ] To prepare the readings to be presented in a mobile app.
 - [ ] To make it so that relevant devices communicate with each other, either by wireless or wired protocols.
 - [ ] To make a good documentation, which gives programmers fast information to use for debugging and configuration.

### Personal requirements
 - [ ] Make use of MKR Wifi 1010 to upload sensor readings (from self or other boards) via MQTT.
 - [ ] Make use of MKR WiFi 1010 to authenticate cards via an online database (could be a local raspberry pi later).
 - [ ] Make use of a knob to have a menu (after login).
 - [ ] Make use of a database and an online API for the MKR WiFi 1010 to communicate with (both MQTT and HTTP).
 - [ ] Send warnings and errors (if possible) to the online API and/or Discord API; Discord API is if there is time.
 - [ ] Make use of the RTC clock and have it synch with the internet (if possible).

#### Components
 - [ ] MKR WiFi 1010 (Board)
 - [ ] RFID-RC522 (RFID Reader)
 - [ ] DS3231 (Real Time Clock)
 - [ ] SSD1306 (OLED Display)
 - [ ] DH11 (Temperature And Humidity Reader)
 - [ ] MicroServo 9G SG90 (Servo Motor)
 - [ ] LEDs
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


