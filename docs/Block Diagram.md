---
title: Block Diagram, Communication Process, Messaging Structure
tags:
- tag1
- tag2
---


## Block Diagram

![Full Team Blocks drawio](https://github.com/user-attachments/assets/6a1368a0-35ca-4a03-a0ee-dbbe892dc35b)

This block diagram defines the general flow of data throughout the subsystem, where the 12V power supply and UART reception and tramissions flow all throughout the daisy chain providing each subsystem with sufficient power and sufficient data. The system starts with the OLED, as it is the subsystem that holds the 12 volt power supply and sends it throughout the daisy chain. It sends the initial data as well, which transports to the sensor subsystem, then to the actuator subsystem, then back, so that each subsystem has access to messages, even if certain messages will only effect some. The OLED will display the actual pressure and target pressure as well as the victory screen when the game is won. The sensor subsystem will include a pressure sensor which communicates pressure back to the OLED and also uses LEDs to notify the user whether the game is off, on, or won. The motor driver subsystem has a pushbutton which will function as the game's victory button, which will flash the sensor subsystem's green LED and create a victory screen on the OLED.

## Communication Process Diagram

![Sequence Diagram of Team Communication drawio](https://github.com/user-attachments/assets/0f1df4b9-7852-4607-a811-f4be9948c96e)



## Messaging Structure

![one](https://github.com/user-attachments/assets/5747d8c7-5825-4226-8d9b-f47d46d050e7)

![two](https://github.com/user-attachments/assets/7c5601f4-95c1-4e4a-a815-621dbcf16888)
