# Prosthetic Arm for Medical and Industrial Purposes

## Purpose
A bionic arm is developed to mimic the movements of a realistic arm such as grabbing and releasing objects with the help of electromyography. The goal is to create a working arm that exceeds the standard degrees of freedom a commercial prosthetic arm normally occupies, can hold relatively heavy household objects, and can be made at an affordable budget.  It is designed as an assistive technology for people who are immobilized due to the loss of a limb. It can also be implemented for industrial applications where automation can work on challenging or dangerous tasks for human labour to handle. This project was presented at a local science fair with my close friend, Umar Ali. 

<p align="center">
  <img src="https://github.com/GrantPau/Prosthetic-Arm-for-Medical-and-Industrial-Purposes/blob/main/Pictures%20and%20Clips/final-arm-design.PNG"/>
</p>
<p align="center">Figure 1: Final Arm Design<p align="center">

## How it Works
The hand is able to operate using an electromyography (EMG) sensor. An EMG sensor measures how much muscle is in use over a certain region in one's body and is based on which muscles are being attached by the three suction cups. After reading muscle movements, the sensor returns an arbitrary value between 0 and 923 where 0 means your muscle is stationary and 923 means your muscle is fully flexing. By taking these values to the Arduino, it can be programmed by telling servo motors to rotate at a certain position based on the arbitrary value. Hence, a working arm is achieved simply by attaching fishing wire to the servo motors so that the main joints in the hand are in motion. Having servo motors positioned at different angles have different tensions on the fishing wire so the prosthetic hand has the ability to be fully open, fully closed, or partially closed. The code is available [here](https://github.com/GrantPau/Prosthetic-Arm-for-Medical-and-Industrial-Purposes/blob/main/Prosthetic_Arm_Code_2.0/Prosthetic_Arm_Code_2.0.ino).

<p align="center">
  <img src="https://github.com/GrantPau/Prosthetic-Arm-for-Medical-and-Industrial-Purposes/blob/main/Pictures%20and%20Clips/arm-test.gif" alt="animated" />
</p>
<p align="center">Figure 2: Prosthetic Arm Gesture Test with EMG Sensor Attached to Arm

## Mechanical Design
To have realistic dimensions of the arm, my hand was measured and sketched using Autodesk Fusion 360 with several modifications. Modifcations include adding holes that allow fishing wire to go through, and proper structures that would support circular motion for each phalanges. One of the goals was to have all joints in the proximal, intermediate, and distal phalanges to function as they are always in use. Once 3D printed, each component is assembled using hex nuts with appropriate bolts. Proper mounts are modelled to allow placements for servo motors and fishing wire. The motors are mounted to the forearm where it is easily accesible by removing three plates connected via velcro straps. Rubber bands are attached to each tip of all the fingers and thumb to ensure a better grip of the item. The entire arm is positioned vertically and is connected to a wooden surface. Screenshots of the prototype and other media are available [here](https://github.com/GrantPau/Prosthetic-Arm-for-Medical-and-Industrial-Purposes/tree/main/Pictures%20and%20Clips).

<p align="center">
  <img src="https://github.com/GrantPau/Prosthetic-Arm-for-Medical-and-Industrial-Purposes/blob/main/Pictures%20and%20Clips/virtual-hand-prototype.PNG"/>
</p>
<p align="center">Figure 3: Virtual Hand Prototype <p align="center">

## Circuit Schematic
A total of 7 servo motors are used to mimic the following components of the hand: pinky, ring, middle, and index fingers, thumb, thumb metacarpal, and the wrist. The motors are supplied by an external 9V battery which is achieved by connecting x6 1.5V AA batteries in series. All the motors are connected in a breadboard which is connected to the forearm mount using velcro. The EMG sensor is attached to the upper part of the forearm and is powered by the 5V supply on the Arduino. All components are connected to their respective signal, as shown below.

<p align="center">
  <img src="https://github.com/GrantPau/Prosthetic-Arm-for-Medical-and-Industrial-Purposes/blob/main/Pictures%20and%20Clips/circuit-schematic.PNG"/>
</p>
<p align="center">Figure 4: Arm Circuit <p align="center">

## Outcome
Based on the criteria, the design performs well. Our arm has 7 degrees of freedom which is over the conventional 6 degrees of freedom seen by commercial prothetic arms, it can hold objects up to 110 grams, and is built under $100 which is budget-friendly compared to other myoelectric arms that sell for over $5000 on the market. Our design can be improved by using stronger servo motors to hold heavier objects, preventing the forearm to wobble when in action, and adding another mount in the forearm for the battery holder so that all the components can be accessible inside the arm. Overall, we had a great experience throghout the process. The elements we learned is undeniably practical as they are useful in other engineering projects.
