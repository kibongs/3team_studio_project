# 3team Studio Project

## Source Sync
When sync source in Windows, apply git config below
> $ git config --system core.protectNTFS false     


## Client
### ALPR
#### ALPR Build Guide
1. Unzip source\client\ALPR\opencv\build\x64\vc15\bin\opencv_world455d.zip to same folder
2. Open source\client\ALPR\OpenALPR.sln with Visual Studio
3. Select Release Mode for configuration of solution project
(if want Debug Mode, needs to install boost package)
4. Build the solution -> ctrl + shift + b  

### WEB
#### Prerequisite
You need to install NodeJS first.
- https://nodejs.org/en/
- Download stable and reliable version.
- Check node and npm version
  > $ node -v, npm -v
- Install yarn
  > $ npm install -g yarn
- Check yarn version
  > $ yarn -v or yarn --version

#### Run web client Step
1. Run internal node server  
   > $ cd source/client/web/src/images/
   > $ node server.js
2. Run react web server  
   > $ yarn start

#### Important Message
If you want to use video or image files,
they must exist in the 'source/client/web/src/images' folder

#### Certification File
1. ROOTCA : source/client/web/rootca.csr
2. SSL_CRT_FILE : source/client/web/localhost+2.pem
3. SSL_KEY_FILE : source/client/web/localhost+2-key.pem


## Server
#### Server URL
- https://team-server-dhzve.run.goorm.io/

#### Server Health Check URL
- https://team-server-dhzve.run.goorm.io/life

#### Server Running Guide
1. Connected Goorm IDE (https://ide.goorm.io/)  
2. Login to Goorm IDE with Google  
   please contact to 3team for google accout information  
3. Start a container ("3team_server")  
4. Enter the command for running server in goorm IDE  
   > $ nohup python server.py &

## System User Info
|ID|Passwork|OTP QR|
|------|----|------|
|test@gmail.com|Qwer!234|![image](https://user-images.githubusercontent.com/107097019/177063393-d32a379a-a696-448b-be66-fed9e73f1bf3.png)|
|test1@gmail.com|Asdf!234|![image](https://user-images.githubusercontent.com/107097019/177063603-66035f8a-3417-4078-9ba9-001107d4c804.png)|
|test2@gmail.com|Asdf!234|![image](https://user-images.githubusercontent.com/107097019/177063622-48a436f6-a637-4b32-973f-fb7a6d1011d5.png)|
|test3@gmail.com|Asdf!234|![image](https://user-images.githubusercontent.com/107097019/177063649-71560ce5-1fc6-4f9f-a7d1-6661f0e2fc03.png)|

#### OTP Step
1. Open Google Authenticator
2. Tap on the + button
3. Then tap on "Scan a QR code"
4. Click Add
