+++
draft = false
comments = false
slug = ""
tags = ["C++", "Robot", "Sensors", "8051", "Microcontroller", "Control"]
categories = ["Robotics"]

showpagemeta = true
showcomments = true
date = 2018-05-21T20:48:27-06:00

title = "Microcontrolled Takeout Robot"
description = "A pneumatic robotic arm powered by an 8051 microcontroller"
externalUrl = "https://github.com/ammarasmro/MicroContolled-Takeout-Robot"
image = "/img/portfolio/microcontrolled-takeout-robot/cool_cover_circuit.jpg"
+++

A pneumatic robotic system that has two movements about two axes, it is used as a take-out robot to carry any object (like a bottle or a jar or anything solid) from one side to the other. Several analysis were carried out to analyze the movements of the robot. The detection of the object can is done by a photo sensor. A strain gauge is installed in the system to detect the weight of the object. The 89c52 microcontroller is used to control the robot movement by controlling the electromagnetic valves. The microcontroller is programmed using C++ language. The sensors are used in a feedback loop to control the termination of the robot. An LCD display is added to display available options for the operator to select, which is done by pressing 4 push buttons, and to display the current state of the robot. The aim of the project was to design the controller, construct a prototype, and display it at the **Design Day** competition at the University of Duhok. Our project placed first on the ECE projects in the competition.


#### Main Parts
* **The robot**
  * *Rotary Cylinder*
  * *Linear Cylinder*
  * *Robotic arm (The grip)*
* **Pneumatic valves**
* **Photocell sensor**
* **Strain gauge**
* **Control circuit**
  * *Microcontroller*
  * *LCD*
  * *Push buttons*
  * *Instrumentation amplifier*

{{< figure src="/img/portfolio/microcontrolled-takeout-robot/final_schema.jpg" width="60%" caption="Schema" >}}

##### The Robot
{{< figure src="/img/portfolio/microcontrolled-takeout-robot/robot_vertical.jpg" width="60%" caption="The Robot" >}}

{{< figure src="/img/portfolio/microcontrolled-takeout-robot/linear_cylinder.jpg" width="60%" caption="Linear cylinder" >}}
{{< figure src="/img/portfolio/microcontrolled-takeout-robot/rotary_cylinder.jpg" width="60%" caption="Rotary cylinder" >}}

{{< figure src="/img/portfolio/microcontrolled-takeout-robot/control_circuit.jpg" width="60%" caption="The controlling circuit -- the main outcome of the project" >}}
