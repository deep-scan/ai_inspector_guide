#**Settings**

The following settings enables the user to configure the process flow, link the cameras and view angles, setup the machine learning detections for the entire process.
The user has full control over how the system flows and captures the data over the entire process.
<br/> 
<br/>

There are 4 sets of configuration settings - 3 of which are in the "conf" folder and 1 within Deep-scan&reg; :
<br/>
A. App Configuration
<br/>
B. Deep-scan&reg; Settings Tab
<br/>
C. Mandatory Process Steps
<br/>
D. Process Steps
<br/>
<br/>





## **A. App Configuration**
In this configuration, the user sets up the process names, part names and links the AI modules to the process step files from the above steps.
<br/>
Open the App.conf file under the Conf Directory.
<br/>
<br/>

### **1. mandatory_process_file**
Enter the directory and filename to match the filename for your Mandatory Process Step file.
<br/>
Mandatory process file link - example:
<br/>
![settings_3.png](settings_3.png)
<br/>
<br/>

### **2. profile**
Enter the profile name of your process in small caps single string. This will be displayed in the User Interface as reference for the assembly Station ID during software operation.
<br/>
Overall profile name of the process - example:
<br/>
![settings_4.png](settings_4.png)
<br/>
<br/>

### **3. stations**
The name on the left of “=” needs to match the profile name. The names of the config files after the “=” needs to match the filenames provided to the user during the system purchase.
<br/>
Station name of the process - example:
<br/>
![settings_5.png](settings_5.png)
<br/>
<br/>

### **4. ptzcam zones**
Setup the names for the zones in any alpha numeric string, as in the example below, but the names must be unique and the number indentifier after “=” must be unique.
<br/>
PTZ camera zones - example:
<br/>
![settings_6.png](settings_6.png)
<br/>
<br/>

### **5. photo_capture_with_bbox**
Setup the process photo capture option with either the detection box Yes or No.
<br/>
Photo Capture with detection box - example:
<br/>
![settings_8.png](settings_8.png)
<br/>
<br/>

### **6. camera sources**
Setup the cameras for the system to recognise and connect to.<br/>
USB cameras - use "camera_n" header.<br/>
PTZ cameras - use "ptzcam_n" header. <br/>
"n" is a running number for the user to decide.<br/>
USB cameras are UVC compliant, and PTZ cameras are IP protocol cameras.<br/><br/>
Use the following example as a guide to setup. The IP address must match the PTZ camera's address in the camera's webpage. <br/>
Sources - example:
<br/>
![settings_9.png](settings_9.png)
<br/>
<br/>

### **7. PTZ camera IP address**
Setup each PTZ with a unique IP address. The system uses these unique IP addresses to retrieve the video feed and to control the camera's PTZ actions.<br/>
a. Connect the IP camera directly to the computer's Ethernet port, or through the PoE switch.<br/>
b. Turn ON that particular PTZ camera you wish to setup the IP address, and turn OFF all other PTZ cameras in the system.<br/>
c. Check the current IP address of the camera from its front LED display.<br/>
d. Key in the IP address from the cammera's display onto any web browser. Enter the username and password provided by Oremi at the login page as follows:<br/>
<br/>
![settings_10.png](settings_10.png)
<br/>
<br/>
e. Click on "Configuration" tab, see picture below, under "Network Configure" click on "Ethernet".<br/>
f. Change the last digit of the "IP Address" to your desired value.<br/>
g. Click on "Save" button.<br/>
h. Logout, then power cycle the camera to enable the new IP Address.<br/>
i. Confirm the IP Address change fron the font LED display of the camera after power cycle.<br/>
<br/>
![settings_11.png](settings_11.png)
<br/>
<br/>

### **8. Ethernet settings in Windows**
Assign IP settings for the PTZ cameras.<br/>
a. Type "Control Panel" in Window's "Search" cell beside Window's "Start" button, then click on "Control Panel System" icon<br/>
b. Click on "Network and Sharing Center".<br/>
c. Click on "Change adapter settings".<br/>
d. Double-click on "Ethernet", then click on "Properties" button.<br/>
e. Select "Internet Protocol Version 4(TCP/IPv4), then click on "Properties" button.<br/>
f. Select "Use the following IP address, change the settings to the example below.<br/>
<br/>
![settings_12.png](settings_12.png)
<br/>
<br/>
<br/>
g. Now click on "Advanced..." button.<br/>
h. Set the IP address and Gateway using the following picture as a guide.<br/>
i. Click on "OK", and "OK", and "OK", and "Close" buttons. This closes all Ethernet settings related windows and saves its related settings.<br/>
<br/>
![settings_13.png](settings_13.png)
<br/>
<br/>





## **B. Deep-scan&reg; Setting**
The Settings tab under the Deep-scan&reg; user interface sets up the Work schedule, Data folder, Database transfer protocol and the cameras' crop, PTZ views. 
<br/>

### **1. Deep-scan&reg; Settings Tab**
![settings_7.png](settings_7.png)
<br/>
<br/>

### **2. Run Deep-scan&reg; AI Inspection software**
Click on the **Settings** tab on the User Interface. 
Enter the password, which is provided to you during the software purchase.

### **3. Operation**
Set up the Work schedule, Data folder, Database Protocol under this section.
<br/>
Click on the **Edit Settings** to edit. 
<br/>
**Station ID**: Click on the drop down list to select.
<br/>
**Part Number**: Optional - click on the drop down list to select.
<br/>
The settings for the rest of the items are intuitive and easy to use.
When completed click on the **Submit** button.
<br/>

### **4. Database (Add-on Module)**
Enter the DSN, UserUD, Password.
<br/>
Click on Test Server Connection to check the Connection Status.
<br/>

### **5. Camera Settings**
Click on the drop down list of the camera to select one of the cameras.
<br/>

**5.1 Crop**:
This is for fixed FOV cameras only as it is unneccesary fpr PTZ cameras. Click on the **Select Region** button, which will bring up the video feed from the camera in a separate window.
<br/>
Left click-&-hold the mouse onto the left-top of the crop area in the video feed window, drag the mouse to the bottom-right of the crop area and release. This will set the crop area of the video feed to the system. Do the same for each camera you wish to crop. 
<br/>

**5.2 PTZ Presets**:
First select the camera from the Camera drop down list.
<br/>
Then click on the Zone drop down list to select the PTZ zone to set.
<br/>
Click on **Set Preset**, this will bring up the video feed from the PTZ camera with the previously saved camera view angles and zoom.
<br/>
Left click-&-hold the mouse, drag the mouse in any X Y direction to position left-right the camera angle, then left go of the mouse button.
<br/>
Scroll the mouse wheel to zoom in-out the camera zoom level.
<br/>
The camera is on auto-focus at all times.
<br/>

**Save PTZ Zone**: Click **Set Preset** to Save the PTZ zone.
<br/>
Repeat the above process for all cameras.
<br/>
Re-start Deep-scan&reg;.
<br/>
<br/>


## **C. Mandatory Process Step**
Open the Mandatory Process step file, see the picture below.<br/>
Fill up just 1 row for the overal process part number. The process is the same as with the Process Steps Settings.<br/>
<br/>
Mandatory process step - example:
<br/>
![settings_2.png](settings_2.png)
<br/>
<br/>

## **D. Process Steps**
These settings configure the process flow for the AI Inspector and link the camera sources, camera PTZ zones and various action items to each of the process steps.
<br/>
Open the Process Steps file under the Conf directory.
<br/>
<br/>
Process step settings file - example:
<br/>
![settings_1.png](settings_1.png)
<br/>
<br/>
Fill up the key process columns in the sheet, as shown in the example below.
<br/>
<br/>

### **1. Detection Classes**
Enter according to the classes provided for each of your parts from the machine learning process.<br/>
<br/>

### **2. Step Number**
This may be in single or multiple decimal points, but it must be unique and prefereably in running order for useful reference.<br/>
<br/>

### **3. Part Name**
This is the component's part name related to the particular process step, it is for the user's internal reference use.<br/>
<br/>

### **4. Part Number**
This is the component's part number related to the particular process step, it is for the user's internal reference use.<br/>
<br/>

### **5. Qty**
This needs to be filled in according to your process. AI Inspector will count it.<br/>
<br/>

### **6. Process Description**
Enter according to your process, but keep it succint for better visibility.<br/>
<br/>

### **7. Allow Skip (Y/N)**
Enter according to your process requirements.<br/>
a. If SKIP = **Y**: Step will be allowed to Skip after "Duration" or upon clicking "DONE".<br/>
b. If SKIP = **N**: Skip Step is not allowed, and user must show correct process to the system.<br/>
c. "BACK" button option *only* appears each time a Step is Skipped.<br/>
<br/>

### **8. Zone**
This is the PTZ camera zone to set the camera viewpoint. The zone may be shared with any process step or specific to the process step. The name may be of any alpha numberic format, so long as it matches the zone name in the App.conf file.<br/>
<br/>

### **9. Generate Voice**
Y/N to read the Process Description.<br/>
<br/>

### **10. Source**
Enter the camera ID. This links the cameras to each process steps in the process file.<br/>
<br/>

### **11. Profile**
Enter the profile option - "part", "barcode", "qrcode", "face", "ocr". Availability depends on your module purchase.<br/>
<br/>

### **12. Data Format**
Authentication format of your barcode, QR code or OCR. You may leave it empty if you wish.<br/>
<br/>

### **13. Sequential**
Y/N for the process step.<br/>
<br/>

### **14. Show Skipped Msg**
Y/N for user interface display in the video feed. <br/>
<br/>

### **15. Capture Photo** Y/N**
This enables options for photo capture of the process step. The photo will be saved in the output data file.<br/>
<br/>
<br/>
<br/>
