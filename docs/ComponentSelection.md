---
title: Component Selection
---
Included pictures represent selected components
## PIC
![PIC](https://github.com/user-attachments/assets/be4c6f78-6222-4529-bc9d-f26b3ab9f0c8)

| Pic | Pros | Cons |
|-----|------|-----|
|PIC18F27Q10-I/SO| Same datasheet as labs | Lowest number of extra pins for debugging|
|---| Gull Wing Leads |
|PIC18F47Q10-E/PT| Much more pins for testing | Very small package|

I don't need a large number of pins for the sensor subsystem, and being able to work with the same layout as labs in class is a big advantage. Hence I chose the PIC1827Q10-I/SO
## Pressure Sensor
![Pressure Sensor](https://github.com/user-attachments/assets/602c4c56-786e-4a00-8b41-50bdfd4aa92e)
| Sensor | Pros | Cons |
|--------|------|------|
|5525DSO-SB005GS|Soldering leads|Minimal Datasheet|
|---|Pressure range falls closely with expected results|Price is middle of the range|
|Honeywell SSCMRNN015PA2A3| Very accurate | Priced much higher |
|---| Ample Documentation | Absolute sensor may not work without proper vacuum |

5525DSO-SB005GS provides me with the range of pressures I expect to be working with given our team's current plans. The price allows me to purchase two just in case of damage to one while still leaving room in my budget for the other pieces, and the gauge style sensor should allow for consistent measurements.
