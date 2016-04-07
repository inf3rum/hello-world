UMBRELLA CITY BUILDER GAME ­ SALESFORCE BACKEND WIRING


# Deployment Guide

# Deployment Instructions

1.	Organization of Submission
=====
Submitted Items:

  1. DeploymentGuide­CITY­BUILDER­GAME.pdf : this doc.
  1. src folder
  1. Sample Data Code City­2
  1. Sample Date Code City­1

## Unmanaged package:

  Use the following package to install Lightning app.
  
  https://login.salesforce.com/packaging/installPackage.apexp?p0=04t36000000WSRo
  
2.	Change Details
=====
As part of this challenge following files added and updated: ­

## Visualforce Pages:
Following VF pages are update to support the requirement changes.

-	<b>CB_Home</b>: Showing city map with Quadrants and Blocks.
-	<b>CB_Play</b>: Page showing selected block with Story question and answer options to play.
-	<b>CB_Leaderboard</b>: Showing Game user order by budget with search functionality.
-	<b>CB_Templates</b>: Template supporting dynamic loading of content.

## Apex Classes:
Following apex classes are update (few blank classes provided as part the challenge assert)

-	<b>CB_HomeController</b>: Home controller class holding logic to laod cities and there related records to show on city Map.
-	<b>CB_HomeControllerTest</b>: This class contains unit tests for validating the behavior of CB_HomeController Apex classes
-	<b>CB_LeaderboardController</b>: Class holding method to get the list of all user to show on leader board UI
-	<b>CB_LeaderboardControllerTest</b>: This class contains unit tests for validating the behaviour of CB_LeaderboardController Apex classes
-	<b>CB_PlayController</b>: Class holding logic to play for a selected block. The logic checks if selected block is valid to play or not
-	<b>CB_PlayControllerTest</b>: This class contains unit tests for validating the behavior of CB_PlayController Apex classes
-	<b>CB_TestData</b>: Class holding static method to create test data used by test classes
-	<b>CB_Utils</b>: Utility class holding static utility method used on Home, Leaderboard and Play controller.


Overall code coverage is 92% above.
## Data Model
-	<b>Game User</b>: Added a new rollup field “Blocks Completed”
```
Blocks Completed CB_Blocks_Completed_c	Roll-Up Summary (COUNT User Block)
```
-	**Quadrant**: Added a new field “Sequence” to allow user adding quadrant sequence.
```
Sequence	CB_Sequence__c	Number(18, 0)
```

## Static Resource:
-	**CB_Base (updated)**: Updated CB_Base following two js files:
  * Script.js
  * citymap.js

3.	Application Setup and Configuration
=====
  1.  Use the above give packages to install the application in you org..
  2.	Once you done with successfully installing the application, you can go ahead create some basic data.
  3.	Creating some sample date:
  4.	Launching the app –
  You can launch the game using the “Game” tab.
  **OR**
  If you are logged in the demo org using the credentials provided as part of this challenge. Can use following URL to directly access the app.

  demo+user107@gmail.com
  
  topcoder#123 
  
  https://c.na30.visual.force.com/apex/CB_Home


4.	How does it work?
=====
Refer to the screen cast video for the overall function walk through.

As part of this challenge, the focus is on Home, Play and Leaderboard pages.

## Home
## Play
## Leaderboard


5.	Jing Videos
=====

## Function demo:
## Code Walk through:
## Demo Org Credentials:

