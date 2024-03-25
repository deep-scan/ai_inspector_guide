The following settings enables the user to configure the process flow, link the cameras and view angles, setup the machine learning detections for the entire process.
The user has full control over how the system flows and captures the data over the entire process.
<br/> 

## A. Process Steps
These settings configure the process flow for the AI Inspector and link the camera sources, camera PTZ zones and various action items to each of the process steps.
<br/>
Open the Process Steps file under the Conf directory.
<br/>
Fill up the key process columns in the sheet, as shown in the example below.
<br/>
<br/>

**Detection Classes**: Enter according to the classes provided for each of your parts.
<br/>

**Step Number**: This may be in single or multiple decimal points, but it must be unique.
<br/>

**Part Name**: This is for your internal reference.
<br/>

**Part Number**: This is for your internal reference.
<br/>

**Qty**: This needs to be filled in according to your process. AI Inspector will count it.
<br/>

**Process Description**: Enter according to your process, but keep it succint for better visibility.
<br/>

**Allow Skip (Y/N)**: Enter according to your process requirements.
<br/>

**Zone**: This is the PTZ camera zone to set the camera viewpoint. The zone may be shared with any process step or specific to the process step. The name may be of any alpha numberic format, so long as it matches the zone name in the App.conf file.
<br/>

**Generate Voice**: Y/N to read the Process Description.
<br/>

**Source**: Enter the camera ID. This links the cameras to each process steps in the process file.
<br/>

**Profile**: Part, Barcode, QR, Face, OCR. Availability depends on your module purchase.
<br/>

**Data Format**: Authentication format of your barcode, QR code or OCR. You may leave it empty if you wish.
<br/>

**Sequential**: Y/N for the process step.
<br/>

**Show Skipped Msg**: Y/N for user interface display in the video feed. 
<br/>
<br/>

### Process step settings - example
![settings_1.png](settings_1.png)
<br/>
<br/>

## B. Mandatory Process Step
Open the Mandatory Process step file, see the picture below.
Fill up just 1 row for the overal process part number. 
The process is the same as with the Process Steps Settings.
<br/>

### Mandatory process step - example
![settings_2.png](settings_2.png)
<br/>
<br/>

## C. App Configuration
In this configuration, the user sets up the process names, part names and links the AI modules to the process step files from the above steps.
<br/>
Open the App.conf file under the Conf Directory.
<br/>

**mandatory_process_file**: Enter the directory and filename to match the filename for your Mandatory Process Step file.
<br/>

### Mandatory process file link - example
![settings_3.png](settings_3.png)
<br/>
<br/>

**profile**: Enter the profile name of your process in small caps single string. This will be displayed in the User Interface as reference for the assembly Station ID during software operation.
<br/>

### Overall profile name of the process - example
![settings_4.png](settings_4.png)
<br/>
<br/>

**stations**: The name on the left of “=” needs to match the profile name. The names of the config files after the “=” needs to match the filenames provided to the user during the system purchase.
<br/>

### Station name of the process - example
![settings_5.png](settings_5.png)
<br/>
<br/>

**ptzcam zones**: Setup the names for the zones in any alpha numeric string, as in the example below, but the names must be unique and the number indentifier after “=” must be unique.
<br/>

### PTZ camera zones - example
![settings_6.png](settings_6.png)
<br/>
<br/>

## D. Deep-scan&reg; Setting
The Settings tab under the Deep-scan&reg; user interface sets up the Work schedule, Data folder, Database transfer protocol and the cameras' crop, PTZ views. 
<br/>

### Deep-scan&reg; Setting Tab
![settings_7.png](settings_7.png)
<br/>
<br/>

### Run Deep-scan&reg; AI Inspection software.
Click on the **Settings** tab on the User Interface. 
Enter the password, which is provided to you during the software purchase.

## Operation
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

## Database (Add-on Module)
Enter the DSN, UserUD, Password.
<br/>
Click on Test Server Connection to check the Connection Status.
<br/>

## Camera Settings
Click on the drop down list of the camera to select one of the cameras.
<br/>

**Crop**:
This is for fixed FOV cameras only as it is unneccesary fpr PTZ cameras. Click on the **Select Region** button, which will bring up the video feed from the camera in a separate window.
<br/>
Left click-&-hold the mouse onto the left-top of the crop area in the video feed window, drag the mouse to the bottom-right of the crop area and release. This will set the crop area of the video feed to the system. Do the same for each camera you wish to crop. 
<br/>

**PTZ Presets**:
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