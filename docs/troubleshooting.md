# **Troubleshooting**
Check out the following Troubletshooting FAQs to resolve your issue faster.
<br/>
<br/>


**1. Video feed is not showing when clicked START**
<br/>
Solutions:<br/>
a. Check if the camera's power is ON, and connected to the computer.<br/>
b. Check to ensure the camera is on Standby mode (Red LED), instead of Booting up mode (blinking Green LED)<br/>
c. Make sure the camera's address in the App.conf file is set correctly, matching the camera's address on its front display.<br/>
d. To check the camera's connection to the computer, use the web brower to access the camera to ensure the camera's functionality.<br/>
<br/>




**2. Object is not detected**
<br/>
Solutions:<br/>
a. Make sure the object is not blocked from the camera angle.<br/>
b. Check the zoom level of the zone, the zoom level may either need to increase or decrease.<br/>
c. Reduce any extreme reflections off the object as this may affect the detection consistency. <br/>
<br/>

**3. Process step in the user interface is not moving**
<br/>
Solutions:<br/>
a. Ensure each process step's descriptions are within 1-row of the Process Guide box. <br/>
Truncate the process step descriptions to contain within 1-row so that the steps are able to auto-scroll within the Proces Guide box's visible range.<br/>
<br/>


**4. Voice guide is not audible**
<br/>
Solutions:<br/>
a. Check that the Generate Voice setting for that process is set as "Y".<br/>
b. Ensure the voice settings in the App.conf file is setting as desired, see below:<br/>

Voice settings in App.conf  - example:
<br/>
![faq_1.png](faq_1.png)
<br/>
<br/>


**5. Camera moves aimlessy**
<br/>
Solutions:<br/>
a. Check Process Step File, ensure PTZ zones set correctly under Deep-scan&reg;, name matches App.conf, zone name and number do not duplicate of another zone.<br/>
b. If the above doesn't work, try install the latest "msvcp140.dll" file from Oremi, in case it is corrupted.<br/>
<br/>

**6. Barcode, QR code or OCR is not detected**
<br/>
Solutions:<br/>
a. Check to ensure the format is correctly set in the Process Step file, make sure the format matches the code read by Deep-scan&reg;.<br/>
b. Make sure the zoom level in the PTZ zone is set sufficiently to have a close enought view.<br/>
c. Reduce the reflections or glare of the code label.<br/>
d. For multiple bar codes within a single camera zone view, let Deep-scan&reg; scan each barcode separately with 5-seconds delay between each label.<br/>
<br/>


**Further support**<br/>
Contact our sales team for further help if the above FAQs do not solve the issue you are encountering.<br/>
<br/>