# Week 10 Activity Log

## Geoserver: install
* followed videos for installation 
* Using Tomcat
* ![image](https://user-images.githubusercontent.com/91274079/159707131-7a6a05eb-11cd-441c-8dd8-69d7f440f721.png)
* ![image](https://user-images.githubusercontent.com/91274079/159707153-4f74c87d-6547-4a50-92a3-6f9576e36dfe.png)

In the setup make sure to check these two boxes
* ![image](https://user-images.githubusercontent.com/91274079/159707271-46f4dbef-57c5-4b79-b083-8231b7a0028b.png)

If you try to open Geoserver (localhost:8080) and see this image you it worked. 
* ![image](https://user-images.githubusercontent.com/91274079/159707373-d0ba7503-84f8-4fc3-b4b9-e40d88629721.png)

Download and extract WAR zip file and put geoserver.war into the tomcat folder created in the installation process. 
* ![image](https://user-images.githubusercontent.com/91274079/159707536-204cb148-28bd-482b-b3ae-914051577d36.png)

Now this should work. 
* ![image](https://user-images.githubusercontent.com/91274079/159707587-38cf2bf0-f33b-417f-91d4-b6d98f01feff.png)

## Geoserver IIS
* Make so IIS can redirect rtraffic from port 80 or 443 into tomcat running on port 8080 on defaut
* Go to Security -> Users, Groups, Roles -> Users and groups -> select admin and then change the password. Save when done. 
* ![image](https://user-images.githubusercontent.com/91274079/159707791-f4b0dd89-1918-47d6-a2be-95d96dca67ca.png)
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
* While liost proxy in the xml doc under web inf. 
* ![image](https://user-images.githubusercontent.com/91274079/159708963-9a90520a-b069-4e2c-81da-cbb0f6a287f6.png)
* ![image](https://user-images.githubusercontent.com/91274079/159709043-6c3f745e-5745-48cd-b090-e4dc0b958a5b.png)

#Running into problems...
* Checked IIS authentication and url rewrite (tested and worked)
* Security
* File priv for geoserver (is this required)
* When it worked I had not done the create new user 
* Removed url rewrite rule, removed proxy base url
* Local works 
* Duckdns works to login then after log in goes to local 
* Redo rewrite rule…. Tested and it works. 
* In shawns video he has https in proxy base url. It might just be http
* It worked! 

## add data to Geoserver
* Copy and paste the canada shapefile from geom 99 lab demos to …/data/data
* Go to workspaces in geoserver
* ![image](https://user-images.githubusercontent.com/91274079/159709740-4c780fe1-c5ef-4e2e-bdca-e1432c378002.png)
* Have workspace now need to connect to data store (allowing multiple shp)
* ![image](https://user-images.githubusercontent.com/91274079/159709796-9af2d805-d76f-4a47-be5d-cf4d269b47a6.png)
* ![image](https://user-images.githubusercontent.com/91274079/159709864-ac708d75-1f30-4d55-94f8-457517bb507c.png)
* Publish the single shp layer
* Make sure to define extent! native and lat/long bounding box
* ![image](https://user-images.githubusercontent.com/91274079/159709922-e91fe5a7-07bf-4813-bcac-5124b8295222.png)
* New layer (WFS) in QGIS. get the url to the server. 
* ![image](https://user-images.githubusercontent.com/91274079/159710098-429167d4-cd7b-4d0a-87ad-49bd70410772.png)

# Geoserver: Beaunmont SHP files
* for the purposes of just exploring I am going to convert the layers from BEaumonts rest/services to shapefiles.
* This will NOT be done in the final solution/ collab proj 
* Open layers in map in AGOL, save it, open it in ArcGIS Pro then run this model (created single folder with all the .shp's)
* ![image](https://user-images.githubusercontent.com/91274079/159710711-d98519b9-4a6c-4841-9bc9-442581ca02c8.png)
* followed exact methods as above to 1) create a new workspace Beaumont, 2) create a new store TreeInv (directory of shapefiles), 3) publish
* There is a difference between PRO and Q... 
* Pro mis missing more than half of the trees (n = 3000, so maybe a limit was reached?), whils QGIS has the correct number (n = 7987). 
* ![image](https://user-images.githubusercontent.com/91274079/159711516-455f5139-897b-4ee8-8fce-fba11c055e6d.png)
* ![image](https://user-images.githubusercontent.com/91274079/159711532-b6ed72d4-aaab-49d4-8adb-ec87c22ac573.png)

## NEXT STEPS
* Bring these shps or bring in data another way (postgis)into leaflet and then make a map. 
* Q for meeting: does my geoserver have to be running in order for Shawn to mark it?










