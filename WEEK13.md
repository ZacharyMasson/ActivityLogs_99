# Week 13 Activity Log
* started experience builder for dev in week 12 (having it here to keep it together)

## Experience builder for developers
* Follow https://developers.arcgis.com/experience-builder/guide/install-guide/ for general guide on how to install.
* Installation of ArcGIS Experience Builder https://www.youtube.com/watch?v=BcJxNaKuTxg&ab_channel=ExperienceBuilder
* This video does  decent job, but does not make the npm install clear. 
Following the guide in combination with the video, and keeping in mind to run the node.js command prompt and not the default system one, should be clear enough.
* ![image](https://user-images.githubusercontent.com/91274079/163194861-1029b2fa-d468-42ef-afad-6ca91432269b.png)
* if you see this it works
* opted to not continue with API for offline use (though I tried and it took some time)
* Resolved issues:
* Cant figure out npm install… tried changing settings to get it to recognize the node.js but wouldn’t work. 
* SOLUTION: node.js cmd      (┛ಠ_ಠ)┛彡┻━┻
* CURRENT ISSUES: I am able to create new experiences BUT it seems like I cannot import the beta version for our final solution. 
* This is okay as the developer edition will likely be used for collab and the regular experience builder will be okay.
* IN ADDITION:
		○ See the new experience builder log, but "…it seems like getting the area of the current extent as a VALUE as opposed to something that just influences selection is more of a developers thing" (Me, 2022)
	- Saved as a template and then published
		○ Opened this template in localhost and got this…

![image](https://user-images.githubusercontent.com/91274079/163195392-6d5a3f62-4146-481c-933d-2fd2bd745b1c.png)


## Experience Builder 
* Based on group meetings: Try to find a way to get canopy cover calculated based on extent
* Section and views
* Tree inventory
* Neighborhoods
* Survey request 
* Rework experience builder to have combo of our solutions

New Version with small guides
	1) Keeping same prompt for "welcome to beaumont…"
	- This is likely where we can connect to victors work/ general info on the urban forestry management strategy  (TBD)
	- Intro to the application (TBD)
	2) Main page (Tree Inventory)
		a. This now uses the…
			i. New base data from our client
			ii. New tree inventory 
			iii. Calculated canopy 
		b. New query
			i. Allows the user to select any of the species in the tree inventory to then see the number of trees that fit their criteria (SQL, very simple)
				1) Height is at least…
				2) DBH is at least…
		c. Spatial filter
				1) Based on map extent
				2) Based on drawn graphic
		d. Text
				1) Linked to the results of the query
		e. Chart
				1) Linked to the results of the query and uniquely symbolize each species.
		 
		
		
		
		
		
		
		
		
		
		
		
		
		3) Neighborhood/ Park View
			i. New Lists linked to parks and neighborhoods in view. 
			ii. Interctive text linked to the data to calculate canopy for the neighborhood in view. 
				1) it seems like getting the area of the current extent as a VALUE as opposed to something that just influences selection is more of a developers thing
		
		
		
		4) Survey
			i. Created basic survey123 (connected to the map frame to get the tree ID)
			ii. Need to make it so it gets location as well (but since they have asset ID, maybe not nescessary)
			iii. Ability to add an image 
			iv. Should configure the "what is the concern" to be the actual fields in the tree inventory (suckering, vandalism etc…)
			v. 
![image](https://user-images.githubusercontent.com/91274079/163195832-98d9707e-9568-46c8-b4f1-c626b2e0ec3c.png)




