# Smart-Trolley-Device v2 (STDv2)
The STDv2 runs on an ESP32-SIM7000G circuit board that has been flashed with MicroPython
(see [ESP32 flashing and general details](https://github.com/18684092/ESP32-MicroPython) or
[specific developement board](https://github.com/18684092/CAR)

## Part of a larger project
The STDv2 is part of a larger project and turns a dump trolley (a hand pulled cart / barrow) into a smart trolley by transmitting its GPS location to a central server. The user / operator can press a button to order a robot to arrive at the STDv2 location, cancel this command or tell the robot to return to base. In the future the idea is that the robot will automatically known when to arrive, pickup a tray and return to base through the use of Artificial Intelligence (AI).

Version 1 of this device sent/received messages with websockets [Call-A-Robot](https://github.com/LCAS/CallARobot). V2 uses MQTT messaging. There is a sub-project that integrates V2 into the V1 system [CAR Forwarders](https://github.com/18684092/CAR-Forwarders) by listening to MQTT messages and forwarding to a Websockets server (and visa-versa).

## Repo Files
The files contained within are uploaded to the ESP32 with a fuller description within the [Wiki](https://github.com/18684092/Smart-Trolley-V2/wiki)
