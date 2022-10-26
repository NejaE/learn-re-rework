---
title: "Getting Started"
permalink: noetic_overview_need_to_know
group: "quick start"
rosver: noetic
nav_order: 1
nav_exclude: false
---

# Getting Started

## Requirements

This is a list of all you'll need in order to get Ubiquity robots up and running.

#### ➤ [2x 12V Lead Acid Battery](noetic_overview_batteries)

The robot requires **2X 12V** lead acid batteries and typically we recommend one of the choices in this section:

| Battery Size      | Capacity (Ah)  | Runtime (hours)  | Notes |
| ---------------- | ---------------- |---------------- |----- |
| 1250/1255  | 4 - 6      |      3 - 4		 |	Used when portability of the robot is at a premium - for example if you are travelling by air with the robot. |
| 1270  		  | 7 - 10    |   6 - 8  	 	 |	This size battery makes the robot still light enough to lift. |
| 12350  		  | 30 - 35     |   24+  	 	 |	Recommended only for those who must have extraordinary endurance. This sized battery makes the robot sufficiently heavy that it will be difficult for most users to lift. |

The batteries are commonly available online (https://www.batterysharks.com/) or in local stores that supply products for scooters, wheelchairs, uninterupped power supply systems or even automotive.

NOTE: The provided charger is specified for LEAD ACID BATTERIES ONLY and will NOT work or could even pose risks with other battery technologies. We provide styrofoam inserts with the robot to fit the above battery sizes. Do not discard these styrofoam inserts with the packaging.

#### ➤ [CR2032 Coin Battery](noetic_overview_batteries#the-real-time-clock-battery)

To power up the real time clock and make sure robot time is always accurate. It's a standard coin battery used for a large variety of household appliances like clocks and kitchen scales, broadly available.

#### ➤ [Wifi and SSH Capable Computer](noetic_quick_start_connecting)

Most of the live administration to the robot is normally done by opening an SSH console to the host computer. As such you need what's likely to be a laptop and a capability to run SSH (via Terminal on Mac and Linux or through puTTY on Windows). 

Note: Not required for Conveyorbot.

## EZ-Map

I've you're using EZ-Map and a LiDAR sensor, [continue with EZ-Map set up](noetic_ezmap_intro).

## Conveyorbot

If you're using the Coveyorbot package, which includes the tower and fiducial markers, [continue with Conveyorbot set up](noetic_conveyorbot_intro).

### For advanced use:

Note: Only continue with this if you intend to get more involved with the stock magni, it's not required for the average user.

#### ➤ [Linux compatible computer or virtual machine](noetic_quick_start_workstation)

The Magni robot is normally running all the software for whatever sensors and navigation mode you are using for your project, but as viewing data through a terminal is very limited, it is handy to have a proper ROS workstation so you can visualize the data on your workstation using RViz and run more demanding nodes locally that can then interact with the robot through ROS.
