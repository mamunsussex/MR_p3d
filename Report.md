# MR_p3d
A Report on ‘Quest Game’

Requirement & Deliverables
A 3D game: Having a two storied building, Custom TPC, Spawn concept.
A video: TPC should explore the building by 30 sec, completing (or failing, or both) the game by TPC, must include some object(s) spawn and pick up by TPC.
A Report: 1500 words, Contain storyline/narrative, Plan, Design documents, Script, Research, Criticism of the production.
Appendix: Source code, Assets and resources, Scripts etc

## Introduction

Introduction & Motivation:
Natural elements with a vast firm landscape could encompass positive feeling in virtual world. Usually, the games reinforce us to deal challenging milestones. Considering the competitive attitude a game could be relaxing by involving with natural element. In this game a low-poly version of garden and orchard environment has been used and created so that gamer will pass their time with some elements and feel connected with natural environment. As main task of these game is finding some fruits, it has been named as ‘QuestGame’. 

Concept and Game Story: 
The game converges an idea as per requirement where the gamer will collect and pluck fresh fruits from a firm house as quick as possible through TPC within time limit. The occurrence place of the game is the adjacent vegetable garden and orchard of a two-storied building. There could have dozens of vegetables, fruits grasses, herbs and plants has been grown together. But the gamer will find and pull fruits from four trees and this process will act as like collecting spawn.  
When the main game will be started from a newly designed two-storied building. The gamer will try to be going out by pressing ‘e’ button (here, ‘e’ stands for enter) through a door of a the two-storied building) the TPC will enter the orchard area and find a landscape view of form house. After pressing ‘e’ button the timer will be activated and count down will be started and a task list will be displayed in the left side of the screen. Then the gamer responsibility is finding the four trees from the orchard and garden area. The trees are Green Apple, Orange, Mango, and Jack-Fruits. Though the firm house is full of vegetables, fruit trees, grasses, herbs, and flowers etc. After reaching a fruit-tree and collecting a fruit a specific task will be completed. By collecting all given fruits, the game will be ended successfully. If the gamer fails to collect all assigned task within time limit, he/she/they will be getting message showing failure and it could be restarted by pressing ‘R’. And thus, try to complete the assign tasks.


### Design
 
Figure: Primary Sketch
 
Figure: UML Class Diagram
 


## Script

The game contains two script files, One for developing the logic to detect the collider box and another one has been worked for how the game manager logic is functioned. In this code, there are two types of functions: some are unity in-built, and some are customized. The functions used in the script have been mentioned below:

Start()-> 		unity built in function, starts on the first frame,
Update -> 		unity built in function, is called on every frame
OnTriggerEnter -> unity built in function to check if the player is on the detection area
OnTriggerExit -> 	unity built in function to check if the player is out of thr d			etection are
HandleTimeup()-> 	custom function that takes care of the logic after the time is up
StartTimer-> 	custom function that starts the timer.
SetChecklist-> 	custom function, keeps track of the items

## Implementation

Implementation Process from High level:

Design custom 3d models.
Import ready-made 3d models and create new ambience.
Default TPC import.
Replace the default TPC body with new skin
Script writing.
Scene Development.
Improve the environment.
The details of these are given below:

a)	Design custom 3d models: A few dedicated 3D models have been designed for this specific game. Among these, the two-storied building is notable as per the requirement. The two-storied building was designed in Cinema 4D software and exported in FBX format to be usable in Unity 3D software. Apart from the building, the main object spawns, the four fruits are customized and designed. It also includes a special fruit Jack-fruit, which contributes to the unique value addition of the game. Three other models are also self-made, which are used in the game.
b)	Import ready-made 3d models and create new ambience: Apart from customized 3D models, ready-made 3D assets are used here. Collect this asset named 'Polyfarm'(External link) from an external source (from this link). However, very little of the peripheral assets are used in the core activities of the game. Basically the models of trees, grass, vegetable field, forest, farm house road, cloud, sky etc. are used in this asset to create a believable ambience and convey the landscape. It can be said that these are the passive part of this game. However, most of these assets are not fully utilized. Several redesigns and position re-placements have been made.
c)	Default TPC import: The third Person Character Controller starter asset is available in the Unity Asset Store and is configured to use in the game scene with a re-configuration. To do this, I had to download and import the default Third-Person Character Controller first. Then I had to configure the Player active Input Handling Settings. To launch the 3rd Person Character Controller, had to drag PlayerArmature into the scene and it can be controlled with the WASD keys for lateral movement and the Space bar for jumping.
d)	Replace the default TPC body with new skin: There are several steps to replace the default TPC which basically looks like a robot. For this, initially an external avatar is downloaded from the SketchFab (https://sketchfab.com)site. The downloaded skin is then rigged from the mixamo (https://www.mixamo.com) site. Rigging mainly applies the movement and kinetics of harvesting fruits from trees. This has made it possible to add new TPC or human like avatars to the scene.

e)	Script writing:  The scripting of the game is divided into two parts. One developed the logic to detect the collider box. In the other, the game manager logic is created. In particular, functions related to counting time, starting and ending time have been added to the game manager script. In this part the logic is scripted for how many tasks are successful and unsuccessful according to the assigned task. Activating successful pickup operation through UI is also done.

f)	Scene Development:  A key part of scene development work is locating and relocating game objects and models according to plans. Especially since spawn objects such as trees and fruits are isolated and separate, they have to be visually logical. That is, isolated fruits are served hanging from the tree.
The next step in scene development is to set colliders to two-story buildings and trees actively involved in the game. Because the output generated in Cinema 4d did not include collider boundaries, TPCs often ran into other meshes such as walls, stairs, windows, etc. As a result, colliders have to be added to each mesh according to the logic of physics like real objects.
An invisible box collider is set in the tree area to simulate the scene of harvesting fruits. Harvesting will be triggered when the TPC or avatar reaches the radius of this box. Finally the imported assets are redone and relocated and the environment is improved and customized.

## A Research Element

Apart from the class material, this project introduced several new topics. Character rigging is notable among these. This task is accomplished very minimally with Adobe Corporation's Maximo Web Application. But the site seems interesting for character interaction design in future games.
Also had to work on modeling fruits and buildings from scratch with Cinema Ford. Many of which have to be studied and explored.

## Summary

Critic of QuestGame
As a game it is very basic and every component needs to add value to make it to production level. Contribute the most to ideas. The idea of collecting fruits from trees only within the limitations of a timer can seem monotonous at times. However, as a single-man effort, this is a prototype that may reach production level in the future.
Problem Encountered and Solutions: At first, I have modeled the the two-storied building with Cinema 4d instead of pro builder. At beginning of the lab work I have encountered some issues to install the academic version of Unity 3d. Currently I have solved the issue by installing the free version in mac properly.
Environment Setup: To create the 3d Games I have to use Unity 3d for scene development and game build. Additionally, I have used Cinema 4d for creation custom models

## Future Work

This game production could be considered as a prototype or minimal viable product (MVP)। The game has several limitations that may be added in the future. Notable among these are:
1. Adding scenes of making salad platters with harvested fruits.
2. Adding pointers to spawns. Adding variation of points according to different categories.
3. Build a customized farmhouse. Especially adding more elements to Amiens.
4. Making low-poly models more realistic.
5. Further improving the timer, dashboard, instruction graphics and UI.

Acknowledgement: I am acknowledging various online resources and some members of the online forums/groups for suggesting Maximo and PolyFirm assets. 

## Appendix A

A link to GitHub repository: https://github.com/mamunsussex/MR_p3d 
A link to Microsoft Onedrive: [MR_P3D_Final](https://universityofsussex-my.sharepoint.com/:f:/r/personal/mr753_sussex_ac_uk/Documents/MR_P3D_Final?csf=1&web=1&e=dOTmRK)
B. scripts: Attached 
C. References to any assets used 
1. https://assetstore.unity.com/packages/3d/environments/industrial/polygon-farm-low-poly-3d-art-by-synty-146192
2.  https://sketchfab.com
3.  https://www.mixamo.com
 



