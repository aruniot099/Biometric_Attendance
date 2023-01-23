# Biometric_Attendance

1.  Download Codes from svn co https://github.com/Sekharjala/Biometric_Attendance

2.  Create a google sheet using a gmail account.

3.  In the google sheet go to Extentions --> Apps Script

4.  Navigate to codes Folder and Copy the code from codes/script.txt and paste it here 
                
                i.      Modify the script as per requirement.
                ii.     Enter google sheet ID from the url (In the url https://docs.google.com/spreadsheets/d/1HmAt-XYZPdbXcZaNz-E5_cYHCfFtOL9dNTZjzSKqHDQ/edit#gid=0  only 1HmAt-XYZPdbXcZaNz-E5_cYHCfFtOL9dNTZjzSKqHDQ is google sheet ID. )
                iii.    Enter google sheet Name.
                iv.     Deploy the code and give nessary permissions.
                v.      After Deployment we can see a google script url and google script ID.Make a note of this for editing purpose in later steps.
 
 
                 
Ubuntu OS:

5.  Install PLatformio  on Terminal using  pip3 install platformio

6.  Navigate to codes folder and edit src/main.cpp 

7.  Edit  WIFI crentials and google scripts as per the requirment.

8.  Generate bin file using : pio run (or) sudo pio run

9.  upload the bin file on Esp32  using : pio run -t nobuild -t upload (or) sudo pio run -t nobuild -t upload

10.  Connect the circuit as per the codes/pin_connection.xlsx.

