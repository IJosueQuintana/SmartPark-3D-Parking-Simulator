# SmartPark — 3D Parking Simulator

SmartPark is an academic project developed for the **Computer Graphics** course at **Escuela Politécnica Nacional (EPN)**.

The project implements an interactive 3D parking environment that combines real-time graphics, vehicle simulation, parking-space management, route calculation, network communication, and integration with a mobile application.

The complete system integrates a **C++/OpenGL 3D simulator**, a **Python backend**, and a **Flutter mobile application**.

> **Academic collaborative project:** SmartPark was developed as a team project. This repository is part of my personal portfolio and documents the system and my individual contributions. The original source-code repository is maintained privately by the project team.

---

## Project Overview

SmartPark was designed as an integrated parking simulation and management system.

The 3D environment allows a user to drive a vehicle through a multi-level parking facility while the system manages parking-space states and provides navigation toward available spaces or the parking exit.

The project combines concepts from computer graphics, algorithms, networking, software development, and real-time system integration.

### Main components

* 3D parking simulator developed with C++ and OpenGL.
* Vehicle movement and driving simulation.
* Multi-level parking environment.
* Parking-space management.
* Route calculation using graph-based navigation.
* Python backend for communication between system components.
* Flutter mobile application.
* Real-time state synchronization through network communication.

---

## 3D Simulation

The main simulator was developed using **C++ and OpenGL**.

The environment includes a multi-level parking structure and provides interactive vehicle control and visualization.

Implemented features include:

* Real-time vehicle movement.
* Forward and reverse driving.
* Steering behavior.
* Braking and friction.
* Wheel rotation according to vehicle movement.
* Steering-wheel angle representation.
* Vehicle behavior on ramps.
* Vehicle inclination according to terrain.
* Multiple camera perspectives.
* Day and night visualization modes.
* Lighting management.
* Parking-space visualization.
* Collision detection.
* Interaction with the parking environment.

The vehicle movement logic considers parameters such as acceleration, maximum forward and reverse speed, braking, friction, steering angle, and wheelbase to produce consistent movement inside the simulation.

---

## Camera System

The simulator provides different perspectives for navigating and observing the environment:

* Free Camera.
* Third-Person Camera.
* Driver Camera.

These modes allow the user to interact with the parking environment from different viewpoints during the simulation.

---

## Vehicle Controls

The simulator supports both keyboard and gamepad input.

Keyboard controls provide the basic vehicle operations required to navigate the parking environment.

Gamepad support allows vehicle actions to be controlled using analog sticks, triggers, and buttons, providing an alternative interaction method for the simulation.

---

## Parking Management

SmartPark maintains the state of parking spaces within the environment.

A parking space can have different states, including:

* Available.
* Occupied.
* Reserved.
* Disabled.

The system can perform operations such as:

* Search for an available parking space.
* Reserve a specific parking space.
* Select an appropriate parking space.
* Cancel a reservation.
* Occupy a parking space.
* Release a parking space.
* Simulate parking-space occupation.
* Search for the parking exit.

The parking-space state is shared with other components of the system to maintain consistent information.

---

## Route Calculation

The parking environment is represented internally using a graph.

SmartPark implements **Dijkstra's algorithm** to calculate navigation routes through the parking facility.

The routing system can calculate paths:

* From the vehicle position to a selected parking space.
* From the vehicle position to the parking exit.

This component applies graph and shortest-path concepts to navigation inside the 3D environment.

---

## Collision System

The simulator includes collision handling for different elements of the parking environment, including:

* Walls.
* Parking boundaries.
* Ramp separators.
* Entry and exit areas.
* Other structural elements of the environment.

Vehicle movement is evaluated incrementally to improve collision handling and reduce the possibility of crossing obstacles when the vehicle is moving at higher speeds.

---

## System Integration

SmartPark integrates several software components rather than operating exclusively as a standalone graphical simulation.

### 3D Simulator

Developed primarily with:

* C++
* OpenGL
* GLFW
* GLM

Responsible for vehicle simulation, graphical rendering, parking visualization, interaction, cameras, and environment behavior.

### Backend

A Python-based backend provides communication services between the simulator and external components.

The system uses network communication mechanisms including:

* HTTP.
* WebSocket.
* UDP-based local network discovery.

These mechanisms allow parking information and system state to be exchanged between components.

### Mobile Application

The project includes a mobile application developed with **Flutter**.

The application can display information associated with the parking system, including:

* Parking map.
* Current floor.
* Vehicle position.
* Vehicle orientation.
* Vehicle speed.
* Selected parking space.
* Calculated route.
* Remaining distance.

This allows information generated by the simulator to be represented on another client in real time.

---

## Technologies

### Programming and development

* C++
* Python
* Dart
* OpenGL
* Flutter

### Graphics and simulation

* GLFW
* GLM
* stb_image
* Blender

### Communication

* HTTP
* WebSocket
* UDP
* TCP/IP

### Development tools

* Visual Studio
* Visual Studio Code
* Git
* GitHub

---

## My Contributions

SmartPark was developed collaboratively. My main responsibilities were focused on the vehicle simulation and interaction components, while I also participated in the organization and integration of the overall project.

My contributions included:

* Implementation of vehicle movement logic.
* Forward and reverse movement.
* Steering behavior.
* Vehicle braking controls.
* Visual wheel rotation according to movement.
* Integration and handling of the 3D vehicle model.
* Implementation and adjustment of camera systems.
* Keyboard controls for vehicle interaction.
* Xbox controller/gamepad support.
* Integration and testing of vehicle behavior within the parking environment.
* Participation in technical decisions and project ideas.
* Coordination and organization of tasks within the development team.
* Collaborative development and version control using Git and GitHub.

Other components of the system, including parts of the parking management, networking, mobile application, and integration architecture, were developed collaboratively by the project team.

---

## Software Concepts Applied

The project provided practical experience with several areas of software engineering and computer science:

* Computer graphics.
* Object-oriented programming.
* Data structures and algorithms.
* Graph representation.
* Shortest-path algorithms.
* Real-time interaction.
* Vehicle simulation.
* Collision detection.
* Network communication.
* Client-server integration.
* Mobile application integration.
* Version control.
* Collaborative software development.

---

## Documentation

The original project includes technical and user documentation describing the operation and implementation of SmartPark.

Available documentation includes:

* User Manual.
* Technical and Source Code Manual.

Because the original project repository is private and was developed collaboratively, the complete source code and internal project documentation are not publicly distributed through this portfolio repository.

---

## Academic Context

**Institution:** Escuela Politécnica Nacional
**Degree:** Software Engineering
**Course:** Computer Graphics
**Academic Period:** 2026-A
**Project Type:** Collaborative academic project

---

## Repository Purpose

This repository is maintained as part of my personal software-development portfolio.

Its purpose is to document the scope of SmartPark, the technologies and concepts applied during its development, and my individual participation in the project while preserving the collaborative nature and privacy of the original source-code repository.
