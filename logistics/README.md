# Logistics Components<img src="https://ramp-eu.github.io/RAMP/img/ramp.png" width="145" align="left">

## Motion Task Planner

[![License: Apache-2.0](https://img.shields.io/github/license/ramp-eu/Motion_Task_Planner.svg)](https://opensource.org/licenses/Apache-2.0)

This Motion Task Planning module computes a motion task plan for the AGVs. This motion task provides a deadlock-free, optimal or near optimal path without loops and collision. Beyond this path computation the Motion Task Planning component handles the communication with the RAN

## Robot Agent Node

[![License: Apache-2.0](https://img.shields.io/github/license/ramp-eu/Robot_Agent_Node.svg)](https://opensource.org/licenses/Apache-2.0)

The RAN (Robot Agent Node) is located between OPIL and the Robot Hardware. It provides two main functionalities: it manages robot navigation, based on ROS, and works as an interface between the robot hardware and the OPIL Cyber Physical Middleware.

## Sensor Agent Node

[![License: Apache-2.0](https://img.shields.io/github/license/ramp-eu/Sensor_Agent_Node.svg)](https://opensource.org/licenses/Apache-2.0)

The SAN (Sensor Agent Node) is located between OPIL and the sensor software and it is a extension of Esthesis platform. It's main features are: 

-   Supports sensors and actuators (Input and output sensors). 
-   Drivers of the sensors and actuators can be written in any prefered/suitable programming language(can use existing drivers), given that at the end the data are sent/retrieved through mqtt protocol, no restriction other than this. 
-   Monitors health of host device(Disk space usage, Memory usage,Restart services, check logs for each running service, Monitor CPU temperature ). 
-   Can be deployed to any host machine that supports java language, eg single board computers like rpi, revpi or any other.

## Task Supervisor

[![License: Apache-2.0](https://img.shields.io/github/license/ramp-eu/Task_Supervisor.svg)](https://opensource.org/licenses/Apache-2.0)

The TaskSupervisor is a system monitor that provides information about the ongoing tasks, as well as their general status


## FIROS

[![License: MIT](https://img.shields.io/github/license/ramp-eu/FIROS.svg)](https://opensource.org/licenses/MIT)

FIROS helps to connect ROS-based robots to the FIWARE Ecosystem, transforming ROS messages into NGSI v2 to publish them in the cloud, and vice versa.


## Human-Machine Interface

[![License: Apache-2.0](https://img.shields.io/github/license/ramp-eu/Human-Machine_Interface.svg)](https://opensource.org/licenses/Apache-2.0)

HMI is a software layer module of the OPIL architecture. It is a web application server with its own local database for storing data needed in this module. HMI serves a web browser user interface for the human agents to monitor and control OPIL data entities.

## Central Sensing and Perception

[![License: Apache-2.0](https://img.shields.io/github/license/ramp-eu/Central_Sensing_and_Perception.svg)](https://opensource.org/licenses/Apache-2.0)

Sensing & Perception is a software module as part of OPIL. It provides the pose of the AGV inside the built map of the environment in which the AGV is navigating and updates the map with the new sensor readings. Additionally, it can build the map with SLAM (Simultaneous Localization And Mapping) if no map is given initially.


## Local Sensing and Perception

[![License: Apache-2.0](https://img.shields.io/github/license/ramp-eu/Local_Sensing_and_Perception.svg)](https://opensource.org/licenses/Apache-2.0)

The local SP module calculates a pose with covariance of the AGV inside the built map or calculates a pose with covariance of the AGV inside the incrementally built map of the SLAM process and sends a pose with covariance of the AGV to Task Planner, HMI, RAN.

