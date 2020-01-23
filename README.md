# image_delay_gui
January, 2020

## 1. Description
This repository provides a GUI tool for controlling the [Newport delay line stage](https://www.newport.com/f/delay-line-stages) and getting images from Thorlabs camera. This GUI works under the following condisionts:
- Windows 10
- Matlab R2018b
- [DL Series Optical Delay Line Linear Motor Linear Translation Stages](https://www.newport.com/f/delay-line-stages)
- Thorlabs Camera

## 2. Control Window
<img src="https://github.com/ksonod/image_delay_gui/blob/master/gui_matlab.PNG" width="500px">  
  
If you run the DLS_GUI_control.py, a new window displayed above will show up. The window consists of 3 sections:
- CURRENT SETTINGS
- CHANGE SETTINGS
- DELAY SCAN

### 2.1 CURRENT SETTINGS
The section of the Current Settings shows the current values of the position, velocity, and acceleration. You can get the latest value by clicking the Update button. If you click it multiple times, you can see that the delay stage position slightly changes.

### 2.2 CHANGE SETTINGS
The Change Settings section allows you to change the position, velocity, and acceleration. You can type values and click the button placed right to the entry box. Move-to-x button initiates the movement of the stage to the target position. The value in the Current Settings is not automatically updated. In order to know the current stage position, you can click the Update button in the Current Settings section. Change-v and Change-a buttons allow us to change values and automatically update the Current Settings section. If you want to change all values and update the Current Settings, you can click Change-x,v,and-a-at-once button. 

### 2.3 DELAY SCAN
This section allows you to do the automatic scan for several times. Once you specify the initial and final positions and number of steps, you can calculate scan step (s/step) and scan range (s) by clicking the Calculate-time-settings button.  
  
Once you start scanning, you can see the progress of the scan.

<img src="https://github.com/ksonod/newport_delay_stage_gui/blob/master/dls_gui_2.PNG" width="200px">

## 3. Useful References
- Official document of the Newport Delay Line Stage: https://www.newport.com/mam/celum/celum_assets/resources/DL_Controller_-_Command_Interface_Manual.pdf?1
- My another repository: https://github.com/ksonod/newport_delay_stage_basic_python
