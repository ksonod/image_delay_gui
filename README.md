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
  
If you run the gui_stage_camera.m, a new window displayed above will show up. The window consists of 2 main sections:
- Image Acquisition
- Delay Stage Control
The Delay Stage Control section contains 3 subsections:
- Current Settings
- Change Settings
- Delay Scan

### 2.1 Image Acquisition
In this section, an image obtained by a camera is displayed. If you click the Get-an-Image button, you can show the current image on the window. If you click the Scan-and-Get-Images button, you can see an image obtained at a specific stage position and save all images in a created folder "scanned images." 

### 2.2 Delay Stage Control
This section allows you to do the automatic scan for several times. Once you specify the initial and final positions and number of steps, you can calculate scan step (s/step) and scan range (s) by clicking the Calculate-time-settings button.  
  
Once you start scanning, you can see the progress of the scan.

<img src="https://github.com/ksonod/newport_delay_stage_gui/blob/master/dls_gui_2.PNG" width="200px">

## 3. Useful References
- Official document of the Newport Delay Line Stage: https://www.newport.com/mam/celum/celum_assets/resources/DL_Controller_-_Command_Interface_Manual.pdf?1
- My another repository: https://github.com/ksonod/newport_delay_stage_basic_python
