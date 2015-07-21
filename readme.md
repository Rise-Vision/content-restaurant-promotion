# Restaurant Promotion Template ![Build Status](http://devtools1.risevision.com:8080/job/Storage-Client-BranchPush/badge/icon)

## Introduction

The Restaurant Promotion Template was created to display a series of high impact animated promotions that can be easily modified to accommodate your specific message. A preview of the template can be seen here: http://rise-vision.github.io/content-restaurant-promotion/index.html

##Steps to run the events template:##

1. Fork or download the entire content-templates repository.
![alt tag](images/readme-step1.jpg)

2. Modify the files within the restaurant-promotion folder directory to fit your needs. (see below on how to modify specific elements)
![alt tag](images/readme-step2.jpg)

3. Host the entire “restaurant-promotion” folder directory in rise vision storage or your web hosting service.
![alt tag](images/readme-step3.jpg)

4. Copy the link to the index.html file where you have it hosted and insert the url into a schedule. (you can also add this link to the url gadget within a presentation)
![alt tag](images/readme-step4.jpg)


##Directions to modify the restaurant promotion template:##

###Changing the text
The slide text is displayed through the use of the google-sheets web component. To see an example of the layout, please see the example spreadsheet located here https://docs.google.com/spreadsheets/d/1orUHfkuPKI8alfmN7KmZbIGOoOWEWsker4LtjEOzb5M/edit#gid=0

You can use your own public spreadsheet by creating a new spreadsheet in google sheets and then selecting 'Publish to the web..' from the File menu. 

Once published, you will need to take copy the key for you spreadsheet which is the long string of letters and numbers found in the url. An example of this can be seen in the url for the example spreadsheet above. Once you have copied the key, please locate the following code in the events.html file and replace the example key with the key from your spreadsheet:

```<google-sheets id="sheet" key="1WwSkJbyIH4EgVDni9eI65zK95MBv0R5c6JSVXsGEPiE" gid="0" rows="{{rows}}" published> </google-sheets>```

In order to view a private spreadsheet, you will need to obtain an ID from https://console.developers.google.com. This is optional if accessing a public spreadsheet, and is currently set to 'sheet' in the above example.

You can then edit the text within the cells of the spreadsheet and the changes will appear in the display.

####Changing the background image
Open the style.css file and locate the following code for each of the 3 images. The background image can be changed by modifying the url information within the () following background-image to the path of your new logo:

``` .image-1 {
	width:100vw;
	height:100vh;
	position: absolute;
	top:0;
	left:0;
	background-image:url(images/background-1.jpg);```

####Changing the text transition
To change the duration of the transition, open the style.css file and locate the following code for each of the 3 images:
```-webkit-animation:image-1-animation 20s ease-out infinite;
	animation:image-1-animation 20s ease-out infinite;```

The length of the animation can be altered by changing the value in seconds (currently 30s) as can the style of transition (currently ease-out).

####Changing the image transition
To change the duration of the text transition (which should always match the image transition), open the style.css file and locate the following code for each of the 3 text blocks:
```-webkit-animation:text-1-animation 20s ease-out infinite;
	animation:text-1-animation 20s ease-out infinite;```

The length of the animation can be altered by changing the value in seconds (currently 30s) as can the style of transition (currently ease-out).

####Changing the logo
Open the style.css file and locate the following code. Modify the url information within the () to the path of your new logo:

```.logo {
	width:10vw;
	height:5vw;
	position: absolute;
	right:4vh;
	bottom:4vh;
	background-image:url(images/logo-onthego.png);```

## Built With
actual tools used
- HTML
- CSS3
- Google Web-Components


Restaurant Promotion Template works in conjunction with [Rise Vision](http://www.risevision.com), the [digital signage management application](http://rva.risevision.com/) that runs on [Google Cloud](https://cloud.google.com).

At this time Chrome is the only browser that this project and Rise Vision supports.

## Submitting Issues
If you encounter problems or find defects we really want to hear about them. If you could take the time to add them as issues to this Repository it would be most appreciated. Please Identify the specific template that has the issue and follow the following format where applicable:

**Reproduction Steps**

1. did this
2. then that
3. followed by this (screenshots / video captures always help)

**Expected Results**

What you expected to happen.

**Actual Results**

What actually happened. (screenshots / video captures always help)

## Contributing
All contributions are greatly appreciated and welcome! If you would first like to sound out your contribution ideas please post your thoughts to our [community](http://community.risevision.com), otherwise submit a pull request and we will do our best to incorporate it.

### Suggested Contributions
- Alternative ways to animate background
- Alternative ways to animate text transitions
- Dynamically update events from custom data source
- i18n Language Support


## Resources
If you have any questions or problems please don't hesitate to join our lively and responsive community at http://community.risevision.com.

If you are looking for user documentation on Rise Vision please see http://www.risevision.com/help/users/

If you would like more information on developing applications for Rise Vision please visit http://www.risevision.com/help/developers/.

 If you have any questions or problems please don't hesitate to join our lively and responsive community at http://community.risevision.com.
 
**Additional Content Templates can be found here: https://github.com/Rise-Vision/content-templates**

**Facilitator**

[Mathew Meiers](https://github.com/mmeiers "Mathew Meiers")
