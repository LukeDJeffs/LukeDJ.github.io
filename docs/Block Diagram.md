---
title: Block Diagram
tags:
- tag1
- tag2
---


## Block Diagram

![Individual Block Diagram drawio](https://github.com/user-attachments/assets/8a280a29-848f-48d7-8d5f-9dec9d603407)

This block diagram defines the general flow of data throughout the subsystem, where the 12V power supply and UART reception and tramissions flow all throughout the daisy chain providing each subsystem with sufficient power and sufficient data. The system starts with the sensor, as it is the subsystem that holds the 12 volt power supply and sends it throughout the daisy chain. It sends the initial data as well, which transports to the OLED subsystem, then to the actuator subsystem, then back, so that each subsystem has access to messages, even if certain messages will only effect some. The OLED will display the actual pressure and target pressure as well as the victory screen when the game is won. The sensor subsystem will include a pressure sensor which communicates pressure back to the OLED subsystem which also uses LEDs to notify the user whether the game is off, on, or won. The motor driver subsystem has a pushbutton which will function as the game's victory button, which will flash the sensor subsystem's green LED and create a victory screen on the OLED.

## Communication Process Diagram

![Sequence Diagram of Team Communication drawio](https://github.com/user-attachments/assets/0f1df4b9-7852-4607-a811-f4be9948c96e)

This diagram defines further the flow of the game, from the start where the sensor system is turned on, all the way to when the pushbutton activates the victory screen and restarts the game. The looping lines reflect the daisy chain connections, as Luke's messages go to Shane's then go to Jack's and then loop back around (if necessary). The initial commands set up the game while the looped commands represent actual game play.

## Messaging Structure

![one](https://github.com/user-attachments/assets/5747d8c7-5825-4226-8d9b-f47d46d050e7)

![two](https://github.com/user-attachments/assets/7c5601f4-95c1-4e4a-a815-621dbcf16888)

These are the messages that will be sent across UART and the daisy chain to each individual subsystem, defined by number and their content. There are multiple types of messages, including the variable pressure sensor value which is designated to 16 bits, then static values indicating a singular state which are only designated to 8 bits. These are the messages that will be sent in the process represented by the communication diagram above.
