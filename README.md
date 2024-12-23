# Heart_rate_detector_project
Metropolia University of Applied Sciences 2024 
This document introduces the evaluation criteria for the technical properties of the Hardware 2 project. In 
addition to these technical requirements, there are also other factors that affect your grade. These include the 
quality of your project report and code. Furthermore, self and peer evaluation results may affect the personal 
project grade. 
This document also includes examples of how the user interface of the device could be constructed on the device, 
including the OLED display. Please note that these example UI images are merely examples, and you are free to 
design the look and use of your user interface in a different way. 
Minimum requirements (grade 1-2) 
• The system must work as a standalone system. 
• The demo must start with an empty system without any libraries installed. 
• The user interface on the OLED screen must have a single-page menu. 
• The device must have an option to start and stop the measurement when the user wants. 
• The device must update and display the updated BPM value every 5 seconds. 
• The calculated BPM values must be possible human heart rate values. 
• The heart rate values must be within +-10% when compared to a reference measurement using a pulse 
oximeter (SpO2 device).
Second level requirements (grade 3) 
• All minimum level requirements must be filled. 
• The device must have a graphical menu with options to choose from. 
• Menu option 1 is for displaying the heart rate the same way as in the minimum requirements. 
• Menu option 2 is for showing basic HRV analysis calculated locally on the Pico board: 
o mean PPI 
o mean HR 
o RMSSD 
o SDNN 
• For the HRV analysis, the device must capture at least 30 seconds of data. 
• The device must connect to the group’s Wi-Fi network and send messages to a client laptop over MQTT. 
• The MQTT broker runs on the Raspberry Pi computer. 
• Basic HRV analysis information is shown on the client laptop. 
Example code for connecting to the Wi-Fi network and publishing MQTT messages on the Pico board can be 
found here: https://gitlab.metropolia.fi/saanapi/hardware-1-networks-final-assignment.
