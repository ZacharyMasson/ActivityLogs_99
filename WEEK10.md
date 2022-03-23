# Week 10 Activity Log

## Geoserver: install
* followed videos for installation 
* Using Tomcat
![image](https://user-images.githubusercontent.com/91274079/159707131-7a6a05eb-11cd-441c-8dd8-69d7f440f721.png)
![image](https://user-images.githubusercontent.com/91274079/159707153-4f74c87d-6547-4a50-92a3-6f9576e36dfe.png)

In the setup make sure to check these two boxes
![image](https://user-images.githubusercontent.com/91274079/159707271-46f4dbef-57c5-4b79-b083-8231b7a0028b.png)

If you try to open Geoserver (localhost:8080) and see this image you it worked. 
![image](https://user-images.githubusercontent.com/91274079/159707373-d0ba7503-84f8-4fc3-b4b9-e40d88629721.png)

Download and extract WAR zip file and put geoserver.war into the tomcat folder created in the installation process. 
![image](https://user-images.githubusercontent.com/91274079/159707536-204cb148-28bd-482b-b3ae-914051577d36.png)

Now this should work. 
![image](https://user-images.githubusercontent.com/91274079/159707587-38cf2bf0-f33b-417f-91d4-b6d98f01feff.png)

## Geoserver IIS
* Make so IIS can redirect rtraffic from port 80 or 443 into tomcat running on port 8080 on defaut
* Go to Security -> Users, Groups, Roles -> Users and groups -> select admin and then change the password. Save when done. 
![image](https://user-images.githubusercontent.com/91274079/159707791-f4b0dd89-1918-47d6-a2be-95d96dca67ca.png)
![image](https://user-images.githubusercontent.com/91274079/159707807-39f814a9-3794-4e9b-b63b-4b0f983ca486.png)

Now use duckdns
* install application request routing https://www.iis.net/downloads/microsoft/application-request-routing
* windows search -> Turn windows features on or off -> Tick IIS sercived checkbox. 
* ![image](https://user-images.githubusercontent.com/91274079/159708258-745dcbb0-ca3a-4b22-8682-486b9df787da.png)
* Enable proxy
* ![image](https://user-images.githubusercontent.com/91274079/159708422-40c192dd-9d0d-4d95-9897-6409ddabd119.png)
* URL rewrite
* ![image](https://user-images.githubusercontent.com/91274079/159708499-e1bcafec-1085-4de5-a124-5c83ebd1b44d.png)
* ![image](https://user-images.githubusercontent.com/91274079/159708522-62b83b06-aa29-465a-ab6d-d5d10aaaca6f.png)




