# Gacha Showcase built on Unity

In this project, there will be several ways to handle a variable system.

.
     Weighted Loot System 
===============================
The first one I've added is the Weighted Loot System, can be found and demo'd on the WeightGacha Scene in \Scenes!
Each category will have a weighted percentage totalling up to 100%. Similar to gacha games now, everything is weighted and in each category will have it's own seperate pool of rewards the random-number-generator gives you.

To interact with the 'Demo', you would start up the scene and proceed to click onto the 'amount' input field. If the UI doesn't seem to be working, please refer to Q1A1 under troubleshooting. You can input two-digit number ranging from 1-99, after the input is typed in, proceed to click on the ROLL icon and the Gacha system will do it's magic and display what you got!

To change the contents and rates of the loot table, you would go to '/Assets/Loot Tables' and inspect the 'Weighted Loot Table' scripted object. In the inspector, you will find that you can add a number of items to it, as long as the total weight is 100. You can change the sprite of the loot, the weight, and as well as the name and so forth.

For now there is an error in terms of the Parallax Sprites having an invalid input.position, but that will not effect the system in anyway but rather the aesthetic and background in the future.

.
     Troubshooting Q & A
===============================
Q1. You've pulled the project and can not seem to interact with the UI?!
A1. This is because of good ol Raycasting and it's priority heiarchy, quite a finnicky little one.
    So to setup the proper Raycasting Priorities, disable the Raycast checkbox under 'Loot Table' Game Object in the inspector.
    If so desired, you can disable all Raycasting properties on all instances. Then the UI of 'Weighted Loot Table' should be 
    then interactable (aka the 'Amount' Area)
    
   
