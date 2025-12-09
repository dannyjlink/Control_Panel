# Control Panel

## Purpose
This is a project to help me keep up with my skills in full-stack PWA development while searching for a new role. Outside of that, the motivation for this is to finally find a use for a 7-inch touchscreen that's been sitting on my shelf for a few years now.  
The goal is to ultimately make a "control panel" for quick actions that wouldn't require me to tab out of whatever I'm doing. Things like muting/deafening on Discord, playing sound clips through my mic, monitoring system resource usage, keeping an eye on my 3D prints, among other things that I'm sure I'll want to add.

## Project Components
There are a few components to this project:
1. 3D printed enclosure to house the screen
- [x] Functional Prototype 
- [ ] Final Version (waiting on filament to arrive)
2. The PWA that will be the UI for the control panel (based on React & Electron, see boilerplate used [here](https://github.com/electron-react-boilerplate/electron-react-boilerplate))
- [ ] System Utilization Display 
3. The backend server to run the actions prompted on the front-end
- [x] System Utilization
    - [ ] Fix GPU Model Names for selection in front-end

#### **This is a non-exhaustive list of planned features that will be updated as the project continues*
  

## File Structure

| Path                  | Key Sub-Directories & Files              | Description                                                                         |
| -------------------   | ---------------------------------------- | ----------------------------------------------------------------------------------- |
| 3D Print & Hardware/  |                                          | .stl files of the enclosure and information on products used.                       |
|                       | Enclosure Files/                         | .stl files of the enclosure parts and assembly.                                     |
|                       | Control Panel BOM.xlsx                   | Bill of materials and products used for this project.                               |
|                       | readme.md                                | Renderings and images.                                                              |
|                       |                                          |                                                                                     |
| Control_Panel_API/    |                                          | ASP .NET Core Web API.                                                              |
|                       | Services/SystemUtilization               | Object oriented C# and C++ code used to poll the system.                            |
|                       | Services/SystemUtilization/GetLUIDS/     | C++ project that gets the lower level hardware information required for some queries|
|                       |                                          |                                                                                     |
| Control_Panel_PWA/    |                                          | React & Electron PWA.                                                               |
|                       | src/renderer/pages                       | Routes within the app.                                                              |
|                       | src/renderer/components                  | Components used within the various pages.                                           |


**This mostly highlights the non-boilerplate files and directories that I worked on.*              