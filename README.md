

# Biometric_Attendance

1.  Download Codes from svn co https://github.com/Sekharjala/Biometric_Attendance/trunk/codes
 
 # Registrations     
      
      i. Register Fingre Prints of Users by connecting the circuit as per pin_connections.xlsx flash the codes/Registrations_FingerPrints.
      ii.Connect the circuit as per the  codes/pin_connection.xlsx.
          *   Install PLatformio  on Terminal using  pip3 install platformio
          **  Flash Esp32 With  codes/Registrations_FingerPrints using (pio run and pio run -t upload).
         

      
# Making Google Sheet to Observe Data
2.  Create a google sheet using a gmail account.

3.  In the google sheet go to Extentions --> Apps Script

4.  Navigate to codes Folder and Copy the code from codes/script.txt and paste it here 
                
                i.      Modify the script as per requirement.
                ii.     Enter google sheet ID from the url (In the url https://docs.google.com/spreadsheets/d/1HmAt-XYZPdbXcZaNz-E5_cYHCfFtOL9dNTZjzSKqHDQ/edit#gid=0  only 1HmAt-XYZPdbXcZaNz-E5_cYHCfFtOL9dNTZjzSKqHDQ is google sheet ID. )
                iii.    Enter google sheet Name.
                iv.     Deploy the code and give nessary permissions.(Deploy--> New Deployment -->(selecttype-->)Web App-->Deploy)
                v.      Authorize Acess and allow gmail permission.
                vi.     After Deployment we can see a google script url and Deployment ID.Make a note of this for editing purpose in later steps.
                vii.    copy Deployment ID and assign  it to google script id in codes/Biometric_attendance/src/main.cpp.
 
 
                 
# Attendance :

5.  Connect the circuit as per the codes/pin_connection.xlsx.

6.  Install PLatformio  on Terminal using  pip3 install platformio

7.  Navigate to codes folder and edit src/main.cpp 

8.  Edit  WIFI crentials and google scripts as per the requirment.

9.  Generate bin file using : pio run (or) sudo pio run

10.  upload the bin file on Esp32  using : pio run -t nobuild -t upload (or) sudo pio run -t nobuild -t upload



