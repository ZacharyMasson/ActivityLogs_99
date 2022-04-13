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

### new version with guide:
 * Keeping prompt for "welcome to beaumont" - TO DO will link to victors scene viewer?, get info graphic on UFMS, write intro to applicaiton
### Main page
 * 	Now uses base data, new inventory, calculated canopy
 * 	new query: allow the user to select any of the species in the tree inventory to then see the number of trees that fit their criteria (SQL v 		easy)
 * 	Height and DBH is ATLEAST
 * 	Spatial Filter: extent or drawn
 * 	Text: linked to results of query
 * 		need to make pretty
 * 	Chart: linked to query and uniquely symbolize 
 * ![image](https://user-images.githubusercontent.com/91274079/163196752-662da2a5-270d-4f81-be56-d93303493ee5.png)
 * ![image](https://user-images.githubusercontent.com/91274079/163196778-57c3530e-1bc6-4e42-bb0d-2ea333df6caf.png)
 * ![image](https://user-images.githubusercontent.com/91274079/163196801-909bbf3e-dd37-4626-af24-f0d6984bf2c7.png)
 * ![image](https://user-images.githubusercontent.com/91274079/163196814-5d40babe-9717-46cb-ad1a-50710d75ea2f.png)

 ### Neighborhood view
 * New Lists linked to parks and neighborhoods in view.
 * Interctive text linked to the data to calculate canopy for the neighborhood in view. 
 * it seems like getting the area of the current extent as a VALUE as opposed to something that just influences selection is more of a developers thing
 * ![image](https://user-images.githubusercontent.com/91274079/163197054-c5bfb2c6-fa10-4a09-909f-e748a6ca25a9.png)
 * ![image](https://user-images.githubusercontent.com/91274079/163197064-d1fb5bc4-5275-4f77-9341-5f4e148a1e30.png)

### Survey 123
* Created a basic survey 123
* needs to get location and tree id
* ability to add image
* TO DO: add conditions to be more like the fields in the actual tree inventory
* ![image](https://user-images.githubusercontent.com/91274079/163197243-b6067fda-7bf6-4407-b9aa-5b903fc0e2ad.png)







