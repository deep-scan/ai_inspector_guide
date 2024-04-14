# **Quick Start**

## **One-Time System Setup**
1. Install Deep-scan&reg; AI Inspector software.
2. Setup the camera(s) by connecting the PoE cable to the computer or power plus Ethernet cable.
3. Setup the inspection or work process steps. 
4. Link the cameras to the process in the configuration file.
5. Setup the AI modules in the configuration file.
6. Run Deep-scan&reg; AI Inspection software.
7. Go to "Settings" tab to setup the Product Part Numbers, Data Folder, Work schedule, Database setup and camera zone setup. 


## **Start using AI Inspector**
1. Run Deep-scan&reg; AI Inspection software. 
2. Click on "START" button on the Main tab. 
3. Follow the process steps as automatically indicated on the user interface.
4. The voice and text prompts will guide the user throughout the processs.
5. Upon completing the process, "PASS" button will light up, click "STOP" to end the process.
6. The data will be saved into the data folder.
7. The camera will self-calibrate upon clicking "STOP".<br/>
The camera calinbration process lasts approximately 30secs, during which a pop-up message will indicate the ongoing process. Once calibration process is completed, the pop-up message goes off automatically and the "START" button is re-enabled.


## **Main Page**
### Navigating the Main Page tab<br/>
1. **START**<br/>
2. **STOP**<br/>
3. **PAUSE/RESUME**: Ad-hoc Pause and Resume for cycle time records. Auto-pause/resume is operational following the work schedule under Settings Tab.<br/>
4. **DONE/BACK**: Click Done to skip the step, if Skip is configured as “Y”.<br/>
5. **Process Guide**: Guide auto-scroll 1-line description.<br/>
6. **STATUS**: Current Status, Report Location<br/>
7. **Detection Table**: Detection and Data results. Scroll to the right for data details.<br/>
8. **Tabs**: Main Page/Settings/Process Setup. Click on Settings, then enter the provided password to enter the Settings Page.<br/>
9. **Parts**: Display All or recent steps’ parts detections. <br/>
10. **Operator**: Display Y/N the operators’ detections.<br/>
11. **PASS/FAIL**: Result of the process. <br/>
12. **Video Feed**: Shows the video feed from the current step’s camera.<br/>
<br/>
*Main Page*: <br/>
![quick_1.png](quick_1.png)
<br/>
<br/>
![quick_2.png](quick_2.png)
<br/>
<br/>

## **Menu**
1. **User Manual**: provides Operations and FAQs, internet access is required.<br/>
2. **Compile Debug Report**: to send the log files along with your issue descriptions to Oremi for technical support.<br/>
<br/>
*Menu*: <br/>
![quick_3.png](quick_3.png)
<br/>
<br/>
![quick_4.png](quick_4.png)
<br/>

## **Settings**
### Navigating the Settings tab<br/>
1. ***Operation***<br/>
a. Data file location - Excel sheet output data including detection time-stamp, cycle time, barcodes and QR codes.<br/>
b. Part number’s list as configured in App.conf.<br/>
c. Operation schedule – self pause and resume over breaks and days (multi-day operations).<br/>
2. ***Database***<br/>
a. Settings for uploads to on-premise sql database.<br/>
3. ***Camera***<br/>
a. AOI crop – select camera then click AOI region in video feed pop-up, click top left corner then drag to bottom right corner which will auto save the AOI.<br/>
b. PTZ zone preset – select PTZ zone, then in the video feed pop-up, left click and drag for pan-tilt, and mouse wheel for zoom. Click “Set Preset” again to save.<br/>
4. ***Overtime***<br/>
a. Set up auto-pause/resume schedule for overtime.<br/>
<br/>
*Settings*: <br/>
![quick_5.png](quick_5.png)
<br/>
<br/>


## **Configuration Setup**
1. ***Configuration files**
a. All configurations files are contained within the “conf” sub-directory.<br/>
2. ***App.conf***<br/>
a. General settings such as displays, dashboard, sound, camera addresses, resolutions etc<br/>
b. Product specific settings such as to link the product part numbers to the machine learning profiles and process steps, camera zones, detection classes.<br/>
3. ***Process Steps***<br/>
a. Product specific process, detection flows and actions.<br/>
4. ***Part Number Detect***<br/>
a. General product model detection.<br/>
<br/>
*Configuration structure*: <br/>
![quick_6.png](quick_6.png)
<br/>
<br/>


## **Display Windows**
1. Individual windows for each camera’s video feed<br/>
a. Video feeds in extended display windows for > 2 cameras setup. For single camera setup the video feed is within the Main Page only.<br/>
b. Size / location configurable.<br/>
2. Visual dashboard<br/>
a. Real time status.<br/>
b. Widget On/Off configurable.<br/>
c. Status cells auto-configured based on process setup.<br/>
d. Work time target setup in App.conf.<br/>
<br/>
*Dashboard window*: <br/>
![quick_7.png](quick_7.png)
<br/>
<br/>

