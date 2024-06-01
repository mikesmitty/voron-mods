# EZ Servo - High Voltage Servo Driver
Turn an unused EZ stepper driver socket on your BTT MMB into a high voltage (6.0V/8.4V) servo output for running high voltage servos with higher torque.

![PCB Render Front](Images/ez-servo-front.png?raw=true) ![PCB Render Back](Images/ez-servo-back.png?raw=true)

### DC-DC voltage converter board for use with EZ stepper driver sockets on the BTT MMB control board
 - TPS5430DDA Step-down converter configured for 6.0V or 8.4V output, up to 3A
 - Pin header with servo output
 - Optionally, use stepper motor output on controller board as servo output (1B: GND, 2B: VCC, 1A: SIG)

Parts that need to be sourced if assembled by JLC:
  - 1-2x 3-Pin Headers [Right Angle Header 2.54mm Pitch](https://www.digikey.com/en/products/detail/molex/0022286030/3158667) or similar 
  - Output Inductor 47uH [Bourns SRP7050WA-470M](https://www.digikey.com/en/products/detail/bourns-inc/srp7050wa-470m/18670339)

```
[servo ez_servo]
# Uncomment the pin for the socket used
#pin: mmb:PB15 # EZ Driver1
#pin: mmb:PD2  # EZ Driver2
#pin: mmb:PD0  # EZ Driver3
#pin: mmb:PB6  # EZ Driver4
```