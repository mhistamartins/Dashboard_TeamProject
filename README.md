## Table of Contents
1. [Introduction](#introduction)
2. [Requirements](#Requirements)
3. [Project Overview](#project-overview)
4. [Tools and Technologies](#Tools-and-Technologies)
5. [Project Architecture](Project-Architecture)
6. [Challenges](#challenges)
7. [Lessons Learned](#lessons-learned)
8. [Demo](#demo)
9. [Questions?](#questions)


# Requirements

- The client and the server shall not depend on a specific communication protocol.
- They shall be able to communicate to each other using TCP/IP and Serial & CAN protocols
- Max. speed is 240 km/h
- Temperature is in the range of [-60, 60] °C
- Battery level in percent.
  
## On the server GUI, there shall be:
- A slider for speed. Speed is an integer in the range of 0 and 240.
- A slider for temperature. Temperature is an integer in the range of -60 and 60
- A slider for battery level. Battery level is an integer in the range of 0 and 100.
- Three checkboxes for the light signals: 
* When left is checked, right shall be disabled and when right is checked, left shall be disabled. 
* When warning is checked both the left.right checkboxes shall be disabled.
* When none of the checkboxes is checked, all of them shall be enabled
  
## On the client GUI there shall be:
- Simple dashboard to display speed, temperature, battery, level, light signals and status of the communication,
- if there is a problem in the communication between client and server.

  
# Project-overview

![Image 2023-09-13 at 10 07](https://github.com/mhistamartins/Dashboard_TeamProject/assets/113973388/91702a55-7b0b-4509-aa5a-b5cb8ef53c6f)


# Tools-and-Technologies

- Version control system / Continuous Integration = Git/Github
> This was used to track changes and collaborate on software development

- GUI design and sound implementation = Qt
> This is a cross platform application for developing graphical user interface.
  
- Project configuration, Dependency management, Builds = CMake, VSC and Platformio
> Cmake is used to manage build process for software projects.
> VSC is a code editor used for code writing and debugging purposes.
> Platformio is an open-source ecosystem for cross-platform development in embedded systems for easier project management for microcontrollers.


# Project-Architecture

![IMG_6267](https://github.com/mhistamartins/Dashboard_TeamProject/assets/113973388/546fc08e-04b4-4af1-ad21-03fd977704a9)


# Challenges

- Technical challenges: members using different operating systems (e.g., Linux, Windows, macOS) presented compatibility issues like sound sync, GUI and Ports.

- Testing complexities: especially when trying to make all functionalities work during CAN communication (supports multi master, message-based protocol)

- Quality assurance: it was difficult maintaining consistent code quality and preventing regression due to frequent updates from various team member, so we implemented a form of continuous integration to avoid conflicts.

- Learning Curve: Learning new tools, frameworks (like Qt), and some technologies during the project was time-intensive and it temporarily slowed down development.


# Contributors:

- [GabeLegendary](https://github.com/gabelegendary)
- [HomajonB](https://github.com/HomajonB)
- [nkkyviv](https://github.com/nkkyviv)
- [Vishnugundu](https://github.com/vishnugundu)
- [mhistamartins](https://github.com/mhistamartins)


# Demo



