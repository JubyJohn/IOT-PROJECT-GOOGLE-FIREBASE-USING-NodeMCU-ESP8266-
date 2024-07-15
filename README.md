# IOT PROJECT: GOOGLE FIREBASE USING NodeMCU ESP8266


## AIM

To create a Firebase project with a realtime database and store and read data from the database using the ESP8266.

## COMPONENTS

1.	ESP8266 NodeMCU
2.	Laser Sensor Module
3.	Buzzer 
4.	Jumper Wire
5.	USB cable

## CONNECTION

### Laser Sensor Module Pin Diagram

 ![Laser_sensor](https://github.com/user-attachments/assets/5d7cd90e-a254-49e9-9830-6250bb4336ae)

<br> S  = Output     ---->  D1
<br> Middle    = power supply  ---->  3V3
<br> GND   = ground   ---->  GND

### Buzzer Pin Diagram
 
![Buzzer-Pinout](https://github.com/user-attachments/assets/caaa4f23-89e2-4d68-ac82-5aa72ad78547)

<br> +  = Output     ---->  D2
<br> -   = ground   ---->  GND


## PROCEDURE

<br> Step 1 : Create a Firebase Project
<br> Step 2 : Interface ESP8266 microcontroller to Arduino IDE using port.
<br> Step 3 : Interface ESP8266 microcontroller with laser sensor to test laser activation
<br> Step 4 : Interface ESP8266 microcontroller with buzzer sensor to test buzzer activation
<br> Step 5 : Install the Firebase-ESP-Client Library.Then, program the ESP8266 to Interface with Firebase
<br> Step 6 : Need to insert your network credentials, URL database, and project API key for the project to work.


### Step 1 : Create a Firebase Project
<br> Set Up a Firebase Account and Create a New Project
#### 1.Create a New Project

<br> -> Go to Firebase and sign in using a Google Account.
<br> -> Click Get Started, and then Add project to create a new project.
<br> -> Give a name to your project, for example: ESP Firebase Demo.
<br> -> Disable the option Enable Google Analytics for this project as it is not needed and click Create project.
<br> Firebase Project Created

#### 2. Set Authentication Methods

<br> -> On the left sidebar, click on Authentication and then on Get started.
<br> Firebase Project Authentication
<br> There are several authentication methods like email and password, Google Account, Facebook account, and others.Set Up Firebase Project for ESP32 and ESP8266 Authentication Methods List
<br> For testing purposes, we can select the Anonymous user (require authentication without requiring users to sign in first by creating temporary anonymous accounts). Enable that option and click Save.Set Up <br> Firebase Project for ESP32 and ESP8266 Authentication Methods Anonymous User

#### 3. Creating a Realtime Database

<br> The next step is creating a Realtime Database for your project. 
<br> -> On the left sidebar click on Realtime Database and then, click on Create Database.
<br> Firebase Project Create Realtime Database
<br> -> Set up realtime database firebase ESP32 ESP8266 Select Location
<br> -> Set up security rules for your database. For testing purposes, select Start in test modeSet up realtime database firebase ESP32 ESP8266 Set Security Rules
<br> Your database is now created. You need to copy and save the database URL—highlighted in the following image—because you’ll need it later in your ESP8266 code.
<br> The Realtime Database is all set. Now, you also need to get your project API key.

#### 4. Get Project API Key

<br> To get your project’s API key, 
<br> -> on the left sidebar click on Project Settings.
<br> Firebase Project Settings
<br> -> Copy the API Key to a safe place because you’ll need it later.
<br> Firebase Project Settings Web API Key
<br> Now, you have everything ready to interface the ESP8266 with the database.


## PROBLEMS FACED

### Error 1 -   Firebase-ESP-Client Library installation
<br> How to rectify:
<br> (1)  Need to find suitable library
<br> (2)  Open above link address -> download ZIP file
<br> (3)  Go to Arduino IDE -> sketch -> include library -> add ZIP file -> downloads -> select downloaded zip file -> close

### Error 2 -   Token info: type = id token, status = on request <br>         Token error: message: is not connected <br>      Token info: type = id token, status = error
<br> How to rectify:
<br> This issue faced because of poor network connection. Try to find a stable network connection and upload.

## OUTPUT

![IMG 1](https://github.com/user-attachments/assets/318e8425-3975-4cad-bdff-37cec63cf75b)

![IMG 2](https://github.com/user-attachments/assets/a3aeb418-a5ef-4acb-8fb9-d41961ed2903)

![IMG 3](https://github.com/user-attachments/assets/f72a6d0d-8a32-4638-b73a-05955acc851d)


## REFERENCES

<br> Google firebase project creation : https://www.javatpoint.com/iot-project-google-firebase-nodemcu
