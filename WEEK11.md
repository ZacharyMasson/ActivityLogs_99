# Week 11 Activity Log

## Story Maps
* Creating a VERY basic story map using the updated web map
* Allow user to go through the different zones and navigate the map
* For the slideshow you  have to make bookmarks for each zone
* ![image](https://user-images.githubusercontent.com/91274079/160676706-35652b71-e5ec-466c-9804-dc22f9286d1a.png)
* ![image](https://user-images.githubusercontent.com/91274079/160676724-9b2893ab-8fc9-4d1c-a1a1-ba90e1fb1461.png)
* No information on the slideshow ( I need to add more text) 
* ![image](https://user-images.githubusercontent.com/91274079/160676956-85e503ac-4ab4-4911-98f2-2d2f3227249d.png)
* Reference Edmonton and Beaumonts Canopy cover and compare


## Geoserver and Leaflet
* NOTE: since geoserver is n ot required for our final solution I am just going to visualize the data on a simple web map and will not update the .shp files created last week. 
* go to this link: https://github.com/iamtekson/leaflet-geoserver-request
* download the ZIP and put it in the same parent folder as the index.html
* ![image](https://user-images.githubusercontent.com/91274079/160677381-12295c68-4555-4652-836d-5672aa2db426.png)
* ![image](https://user-images.githubusercontent.com/91274079/160677395-434c4c49-c781-4f92-93d1-35bac4cccdcf.png)
* Enable JSONP - go to the web.xml file and uncomment these lines
* ![image](https://user-images.githubusercontent.com/91274079/160677487-b290fddc-f522-473d-9f43-eedf9fe286ba.png)
* Use the quick installation method (reference the files directly in the script)
* ![image](https://user-images.githubusercontent.com/91274079/160677611-b1dc8abd-cafc-45a9-b5a1-2fd2a8e11e92.png)
* Navigate to the src folder in the extracted repository and copy the L.Geoserver.js file into a lib folder which is contained in the same parent folder that has the index.html
* ![image](https://user-images.githubusercontent.com/91274079/160677824-6e0a407d-b644-4531-a33f-c5363498c76b.png)
* ![image](https://user-images.githubusercontent.com/91274079/160677832-938c4034-fa41-434a-af63-a6a1499793cd.png)
* in the index.html file (created following the video guide from the repository but heavily simplified and made to have my data), add these lines to 1) get open streetmaps, 2) add the two wms layers (trees and zones)
* ![image](https://user-images.githubusercontent.com/91274079/160678148-eb2b15b7-b556-4639-b752-e49b19e30ba1.png)

* The final product:
* ![image](https://user-images.githubusercontent.com/91274079/160678188-b74c30e5-4192-4a1d-acb5-d63006e002c8.png)

* not going to continue with this since the final solution is more focused on the esri (experience builder/ story map)



