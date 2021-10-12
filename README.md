# Project Robot formation

The Software Part of an affordable Robot for formation Testing or educational purposes.
Implemented is for the ESP32 an Access Point with Webserver Control for the Robot.
Robot has to be build beforehand.


## Requirements:

1. Install Visual Studio Code -> [download](https://code.visualstudio.com/Download) (if not already installed)
2. Install Python [download](https://www.python.org/downloads/) (if not already installed)
3. Install Git [download](https://git-scm.com/downloads) (if not already installed)
4. Start Visual Studio Code -> on the Left side of Visual Studio Code is a button Extensions click on it and search for platformIO ide and install it.
5. open an explorer, navigate to the location you want this [Repo](https://github.com/goldeng0d/SwarmRobotBa.git) to be and open a **terminal/cmd** there. (easiest by clicking into the path and typing `cmd`)
6. Go to the [Repo](https://github.com/goldeng0d/SwarmRobotBa.git) click on Code and Copy the Link ->  for the Repo
7. type in the opened terminal -> git clone <replace-with-link-here>
8. Go Back to Visual Studio Code -> on the Left side of Visual Studio Code is now a Button PlatfomIO click on it and select from Quick Access Open under PIO Home
9. Select Open Project and Select the Folder you just Cloned
10. Download Libraries [lib1](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbFB2Rm56ZWpGbHkybFVVSGVyVG1mb09kb0MwQXxBQ3Jtc0trTU5JQlNnVzBTeXRRd0gtaS1sY3N3Q2NwajM4eWlNQXJITWpHX1ZkWkFzaVZVNnVtck5wYS1BSzBzRl9sQVN0VkhDYUZUTWNNbFFvQUY5elprak1lRDBEOHBTX1k5VWE1WGNkWUV2b2hBeklyUE1nMA&q=https%3A%2F%2Fgithub.com%2Fme-no-dev%2FAsyncTCP%2Farchive%2Frefs%2Fheads%2Fmaster.zip), [lib2](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbGxBbGstb0owX0k2NWpOVmNMMDhoMzNfV3pmZ3xBQ3Jtc0tuaWRyTVpSR1pVSUZrMEZ1di1CMWp3Rm56OU12V1VjLVo1cF80MkYwb0xNM2tBMG9TS1VJbmpSeUlwWGhDSmVGOUVTTExla2VIdTNzTFNNOTFOT3ktUFV1cmxWUG44V3VpRmloQU44Q2djNkhJanBvVQ&q=https%3A%2F%2Fgithub.com%2Fme-no-dev%2FESPAsyncWebServer%2Farchive%2Frefs%2Fheads%2Fmaster.zip) and unzip them
11. Create a folder **lib** on the same level as folder src and move the unzipped libraries into **lib** folder
10. Connect only one ESP32 to your PC
11. On the Bottom Line of Visual Studio Code is a button -> **Switch PlatformIO Project Enviroment** -> make sure SwarmRobotBa is selected
12. On the Bottom Line of Visual Studio Code is a button -> **Upload** press it.
First the Project is build. If the building process succeeds the Upload to the Device is started.
Once Complete Press the RST(Reset) Button on the ESP32.

## How to use:

**important** On a touch Device connect to the 
WIFI: **MyWiFICar** with 
PW:   **12345678**  
open a Browser and search for 
IP: **192.168.4.1**
You See Directional Buttons which are for the Direction the Robot drives.
There is a speed Slider, as well, the Slider is proportional to the max. Speed in percent.


## Upgradeable (ToDo)

- Encoder Reading (Interrupt) with RPM Calculation
- ROS integration for Masters
- Change TCP Server to UDP (for performance)
- Change Access Point to Network Client