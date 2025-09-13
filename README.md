
# MS Canbus Expansion Module
### DIY Canbus expansion module to add more inputs/ouputs to a Micro/MegaSquirt ECU  

### 1. Background
> I am a proud owner of a rusted out 1984 Volvo 242 Turbo which I am in the process of converting to EFI and at the same time rewiring the entire thing because of the original wiring completely disintegrating. 
> 
![Volvo 242 Turbo](https://raw.githubusercontent.com/gabrielHawkins7/ms-canbus-expansion/0a828a86511f689d01d575c2f55159b47fb7b315/images/242.jpeg)
> 
> Originally the car came with K-Jetronic "Mechanical" Fuel Injection which is impossibly complex and before I began this project I had zero prior experience of working on cars, let alone rebuilding one, and the only shop willing to touch this German engineering wizardry of K-Jet was a single shop 4 hrs away from where I live. So I ripped it all out completely and am almost finished converting it to run on Microsquirt using LH 2.2 components from a more "Modern" 240. At the same time I removed every original piece of copper from the car and the amount of sensors available to connect to the new ECU is very limited. Even though the car is completly gutted I'd still like to have some knowledge of oil pressure, oil temperature, fuel level, ethanol content, etc. However, the Microsquirt especially doesn't have enough sensor inputs. This is when I discovered CAN-BUS and had the idea to create my own system to send this sensor data to the MS. 


### 2. Design Goals
- The system must run on a low-power fast startup micro-controller. 
- The system must be able to read and transmit CAN information to and from the Micro/Megasquirt
- The system must be able to read the data from Voltage or Resistive sensor
### 3. Current Progress
 - [X] Select Microcontroller (Arduino Mega due to 5v power requirements) 
 - [ ] Design basic circuit for Voltage/Resistive sensor readings
 - [ ] Implement reading from the MS CAN BUS protocol
 - [ ] Implement sending to the MS CAN BUS protocol
 - [ ] Design physical layout
 - [ ] Design power management system
