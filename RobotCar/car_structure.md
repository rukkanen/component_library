# Robot Car 

Description for the whole project:
The Robot Car project aims to create an autonomous vehicle capable of navigating its environment and capturing images using its movable onboard camera. The project consists of three main components: ARD1, ARD2, and ESP1WS. ARD1 controls the robot's motion, radar, and lights, while ARD2 manages the ESP-01 module and OV7670 camera. ESP1WS is responsible for the web server and camera control. The project utilizes various hardware components, including motors, sensors, and batteries, to achieve its objectives. The robot car's design incorporates a chassis, motors, camera mount, ultrasound radar, enabling it to move, capture images, and avoid obstacles. Overall, the Robot Car project aims to create an autonomous vehicle that can navigate its environment and capture images, showcasing the capabilities of modern robotics and IoT technologies. It's main task is to be idle somewhere and notice with it's microwave radar if someone is approaching. If someone is approaching it will start moving and take a picture of the person. The picture will be sent to a webserver which can be accessed by the owner of the robot car. The robot car will then return to its idle state. Though it can move around from time to time to make sure that the radar can see the whole appartment. THe robot will be in a single appartment it's whole existance.

The robot will make a map of the appartment it is in and store it on a microSD card. The robot will also store pictures of the people it has seen on the microSD card. The robot will be able to move around and take pictures of its surroundings, providing a comprehensive view of the environment. The robot car will be able to navigate around obstacles and reach its destination. The robot car will be able to move around and capture images of its surroundings, providing a comprehensive view of the environment. 

### Milestones
| Milestone | Description |
|-----------|-------------|
| MS1 | Only driving and obstacle avoidance |
| MS2 | ARD2 and ESP1WS |
| MS3 | Navigation based on a map |


## Software Projects
- VS Code with PlatformIO is used.
- ROboCar has three projects:
    - **ARD1** which is the motor, radar and an pathfinder arduino SW project. 
    - **ARD2** which is the ESP-01 and OV7670 Arduino SW project.
    - **ESP1WS** which is ESP-01 webserver (and perhaps picture handling) SW project.

## Arduino Microcontrollers
Two Arduino microcontrollers are integrated into the car's structure using breadboards. These microcontrollers serve as the brain of the car, controlling its movements and processing sensor data. We call them ARD1 and ARD2. ARD1 is responsible for managing the robot's motion, radar, and lights, while ARD2 controls the ESP-01 module and OV7670 camera. The microcontrollers are programmed using C++ and compiled with VS Code and PlatformIO. They are uploaded to the Arduino microcontrollers on the robot car. The microcontrollers are connected to various components, including motors, sensors, and cameras, to enable the robot car to navigate its environment autonomously and capture images. The microcontrollers play a crucial role in the functionality and performance of the robot car, providing the necessary intelligence and control to execute its tasks effectively.

Overall, the physical structure of the robot car is carefully designed to house the necessary components, ensuring optimal functionality and performance.

### ARD1
Controls the robot motion and can function as a pathfinder. It also controls the radar and the lights. This project is written in C++ and is compiled with VS Code and PlatformIO. The project is uploaded to the Arduino microcontroller on the robot car. The project is responsible for controlling the robot's motors, radar, and lights. It also includes a pathfinder algorithm that enables the robot to navigate its environment autonomously. The code for this project will be asked from ChatGPT, and placed in github for both developer and chatgpt to use for further reference.

ARD1 will function as the MWP (minimum working product) for the robot car. It will be able to move around and avoid obstacles. The pathfinder algorithm will be a simple one, but it will be able to navigate the robot car around obstacles. The radar will be used to detect obstacles in front of the robot car, and the lights will be used to indicate the robot car's status. The robot car will be able to move forward, backward, left, and right, and it will be able to stop when it detects an obstacle in front of it. The robot car will be able to navigate around obstacles and reach its destination. This will be MS1 (milestone 1) for the robot car.

The code for this project will be asked from ChatGPT, and placed in github for both developer and chatgpt to use for further reference.

### ARD2
Controls the ESP-01 and OV7670 camera. This project is written in C++ and is compiled with VS Code and PlatformIO. The project is uploaded to the Arduino microcontroller on the robot car. The project is responsible for facilitating the camera connection to the ESP-01 module and controlling the camera's movements. The camera movement is at least at this point done through the webservers web interface
The code for this project will be asked from ChatGPT, and placed in github for both developer and chatgpt to use for further reference. MS2 (milestone 2) for the robot car will be when the camera is able to move around and capture images of the robot car's surroundings. The camera will be able to pan and tilt to capture images from different angles, and the images will be displayed on the web interface. The robot car will be able to move around and capture images of its surroundings, providing a comprehensive view of the environment. This will be MS2 for the robot car.

### ESP1WS
Controls the ESP-01 and the webserver. This project should do as much of the webserver, web serving and camera control as possible since the ESP-01 is already quite a powerful microcontroller. This project is written in C++ and is compiled with VS Code and PlatformIO. The project is uploaded to the ESP-01 module on the robot car. The project is responsible for establishing a web server that allows users to interact with the robot car. The web server provides a user-friendly interface for controlling the robot car and viewing its surroundings through the camera. The code for this project will be asked from ChatGPT, and placed in github for both developer and chatgpt to use for further reference. This is a part of MS2 

## Hardware
**The project can use the following HW (but is not limited to).**
**Dont think that these components must be used, they are here offered only for convenience.**
Some parts must be used, but that's mentioned separately per component.

### Processing components
- 2x Micro Arduino (from now on called ard1 and ard2, like their projects but lowercase)
- ESP-01 8266 breakoutboard (from now on called esp1)

### Robot car kit with 4 motors (3-9 V DC)
- Almost 100% similar to this: https://eu.robotshop.com/products/diy-robot-car-smart-chassis-kit-w-speed-encoder-4w-2-layer-arduino-rpi
- A bigger description can be found behind the link. 
- The motors have discs with holes in them, which can be used to measure the speed of the motors.  
    - "KY-033 IR Infrared Sensor" is used to measure speed

#### Carkit Specifications
- Voltage 4.5 - 9 V DC
- Current in idle state 190 mA
- Engine speed/min in idle 90 - 300 rpm
- Torque in gf/cm min 800 - 1200
- Dimensions (chassis) 280 x 156 x 3 mm
- Dimensions (wheel) 65 x 27 mm
- Car Weight 0.5 kg

### Engine specs (we will almost certainly use the 2x3,7V Li-ion batteries)
| Voltage DC V | Idle current mA | Idle rpm +- 10% | Torque gf/cm min. |
|--------------|-----------------|-----------------|-------------------|
| 4.5          | 190             | 90              | 800               |
| 6            | 160             | 190             | 800               |
| 7.2          | 180             | 230             | 1000              |
| 9            | 200             | 300             | 1200              |

## Power sources

The RoboCar has 4 Li-ion batteries which means that care must be taken to make sure that the batteries dont get shortcircuited and that their heat dissipation is taken care of.
For the Arduino robot, use the MF-R110AP polyfuse (Hold 1.10A, Trip 2.2A) in series with the positive line from the battery to the step-down converters to protect the electronics. For motor protection, use the MF-R400 polyfuse (Hold 4.0A, Trip 8.0A) in series with the positive line from the battery to the motor controller. Additionally, employ a 7.5A automotive blade fuse (ATC-7.5) in the power supply line to the motors. Utilize step-down converters to provide 5V for the Arduino and 3V for the ESP-01. Apply 3M 8810 thermal pads on high-power components for heat management.
*If it turns out that the Li-ion setup is too difficult it must be changed to something else.*

#### Possible polyfuses:
- MF-R90 hold 0.90A trip 1.8A
- MF-R110AP hold 1.10A trip 2.2A
- MF-R135 hold 1.35A trip 2.7A
- MF-R400 hold 4.0A trip 8.0A

### Power for motors
**2x 3,7 Li-ion rechargeable batteries in series (7,4 V nominal voltage, 8,4 V fully charged).**

Two 3.7V Li-ion batteries in series providing a nominal voltage of 7.4V (8.4V fully charged). This setup supports high current supply (5A per cell) and offers a capacity of 2000mAh to 3000mAh. For precise voltage requirements, a step-down converter can be used to regulate the voltage to the desired level. This configuration ensures a stable and efficient power source for the motors.

### Power for Arduino microcontrollers
**2x 3,7 Li-ion rechargeable batteries in series (7,4 V nominal voltage, 8,4 V fully charged).**

The power source for the computers and electronics of the robot car consists of two 3.7V Li-ion batteries arranged in series, providing a nominal voltage of 7.4V (8.4V when fully charged). To meet the specific voltage requirements of various components, step-down converters are utilized: 5V for the Micro Arduinos, 3.3V for the ESP-01 module, and appropriate voltages for other components such as the ultrasound sensor, microwave radar, and LEDs. This configuration ensures a stable 
and high-capacity power supply, delivering efficient and reliable power distribution across all electronic components in the robot car.

## Moving structures, camera mount and ultrasuond radar in front
The robocar is equipped with an HS-SR04 ultrasound sensor mounted on a servo, allowing it to scan the front area for obstacles. This helps the robocar detect and avoid collisions. Additionally, the robocar has an OV7670 camera on a pan/tilt mount, controlled by two servos. This setup lets the camera move around to capture a wide view of the surroundings. These features work together to help the robocar navigate and understand its environment better. Currently there are no plans to use the camera for obstacle avoidance, but it can be used for that purpose if needed. 

## Lights
(Controlled by ARD1)
The RoboCar has a few leds around it to signify that it's active. The leds must be at a very low power not to disturb people around it. Theres a set of leds which show that the car has power and a set of leds which turn on a moment before it start moving and turn off a second after it stops.

The on option to integrate a bright led to the camera which can be turned on by an ambient light
sensor. This can be used to take pictures in dark places.

## What component is connected to what controller or power.
**This info might be wrong!**

| Module       | ard1 | ard2 | ESP-01 | PowerCompute | PowerMotor |
|--------------|------|------|--------|--------------|------------|
| Motors       | X    |      |        |              | X          |
| Radar        | X    |      |        | X            |            |
| Camera       |      | X    |        | X            |            |
| CamLight     |      |      | X      | X            |            |
| Lights       | X    |      |        | X            |            |
| Web          |      |      | X      | X            |            |
| Ultrasound   | X    |      |        | X            |            |
| Ultra Servos | X    |      |        | X            |            |
| NavData      | X    |      |        | X            |            |
| CamServos    |      | X    |        | X            |            |
| MotorSpeed   | X    |      |        | X            |            |
| MotorDriver  | X    |      |        |              | X          |
**something else?**

## Navigation and storing navigation data
The RoboCar is equipped with a SparkFun microSD Transflash Breakout, which allows it to store navigation data and a map. This feature enables the RoboCar to record and save its movements, helping it navigate more efficiently and effectively. The microSD card provides ample storage capacity for storing data, ensuring that the RoboCar can access and utilize the information as needed. By storing navigation data, the RoboCar can enhance its performance and optimize its movements, making it a more reliable and intelligent autonomous vehicle.

## Camera and storing/sending picture
There's a lot of space on the microSD card to store pictures. The pictures can be sent to a webserver which can be accessed by the owner of the robot car. The pictures can be stored on the microSD card for later viewing or analysis. The camera can be controlled through the web interface, allowing the user to capture images of the robot car's surroundings. The camera can pan and tilt to capture images from different angles, providing a comprehensive view of the environment. The pictures can be sent to the webserver for viewing or storage, enhancing the robot car's functionality and capabilities. Put as much of the graphics processing to ESP-01 since it has a lot of power.

## Absolutely all HW components (many might not be needed!)
- 2x Micro Arduino
- ESP-01 8266 breakoutboard
- 4x 3,7 Li-ion rechargeable batteries in series (7,4 V nominal voltage, 8,4 V fully charged)
- RCWL-0516 Microwave Radar Sensor
- HC-SR04 Ultrasound Sensor
- OV7670 Camera
- 2x SG90 Servo Motor
- 1x Pan/Tilt Mount
- A generic micro servo for the ultrasound sensor
- 2x 3M 8810 thermal pads (or similar)
- 2x Step-down converters
    - LM2596 DC-DC Converter Module 
    - XL6009E1 DC-DC Converter Module
    - 1x for 5V for the Arduino microcontrollers
    - 1x for 3V for the ESP-01 module (please notice that ESP-01 is 3V not 3.3V)
- 2x polyfuses
    - MF-R110AP hold 1.10A trip 2.2A
    - MF-R400 hold 4.0A trip 8.0A
- 1x 7.5A automotive blade fuse (ATC-7.5)
    - and holder for it
- 4x motors
    - TI SN754410NE H-Bridge Motor Driver for controlling the motors
    - 4x KY-033 IR Infrared Sensor for measuring the speed of the motors
- 4x KY-033 IR Infrared Sensor for measuring the speed of the motors
    - (called also "KY-033 Line Tracking Sensor Module")
- MPU6050 Accelerometer and Gyroscope Module if needed for navigation
- Perhaps a photoresistor to know ambien light levels for the camera or even wake up for the robot when lights are turned on in the appartment
- Breadboard (17, 30 and 60 row version available)
    - The robocar contain at least one 60-row breadboard
    - We can add very small 17-row breadboards if needed for difficult places
    - @TODO decide what size and which how many breadboards are needed.
- A B10K potentiometer for speed control
- SparkFun microSD Transflash Breakout (for storing nav data and potential maps)
- resistors, leds, potentiometers, buttons and basic components if needed

## General pictures of RoboCard

**Pictures are free to use for all** 

![Photo of a chassis](11_chassis.jpg)
![Photo of a chassis](1_chassis.jpg)
![Photo of a chassis](2_chassis.jpg)
![Photo of a chassis](22_chassis.jpg)
![Photo of a chassis](3_motor.jpg)
![Photo of a chassis](4_corner.jpg)

## Placement of components in the robot car chassis
| Component              | Placement                                                                                           |
|------------------------|-----------------------------------------------------------------------------------------------------|
| Ultrasound servo swivel| Positioned at the absolute front of the car, ensuring optimal scanning capabilities while minimizing the risk of damage in case of a crash. |
| Camera                 | Mounted behind and above the ultrasound radar, allowing for a clear view of the surroundings. The camera is installed on a pan/tilt mount, enabling flexible movement and capturing a wide range of angles. |
| Microwave radar        | Located in the middle of the car, positioned above all other components. This placement ensures accurate detection and avoids interference from other elements. |
| Batteries              | The two (2x18650) battery racks securely hold the batteries, providing a reliable power source for the car. The batteries are strategically placed for easy access and efficient power distribution. |
| Fuses                  | Placed as close to the batteries as possible, the fuses serve as a protective measure, safeguarding the electronics and motors from potential damage. |
| Step-down converters   | Positioned near the batteries, the converters regulate the voltage to ensure optimal performance of the Arduino microcontrollers and ESP-01 module. |


