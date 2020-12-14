
Final Project

CS 425-001

Team members: Alexander Gobs

Game name: Simple Slash and Shoot


I tried adding the files for the game but the filepaths were too long for github to handle so I had to give up on that.


1.	Provide an overview of your game (give a short description about the game, i.e., core mechanics, game plot, objective, etc.): 

I made a small bullet hell kind of game. The player starts in a room and enemies will come from the manholes near the sides and attack the player. The player has a sword and a gun to fight back the enemies.
The objective of the game is for the player to get as many kills as possible before dying in order to get a high score.


2.	What will be the main technical components (game AI, motion planning, physics, procedural content generation) that your game will focus on? 

The game uses behavior trees and AI to help choose what the enemies will do.

I implemented selector nodes, sequence nodes, and action nodes.

For example, the enemies will run away from the player and go back to the manhole they came from if their health falls below 1/3 of their health.
If their health is not below 1/3 of their max, then they can try shooting at the player
If shooting at the player fails, then they will charge towards the player.

This allowed me to do both enemies AI in a single behavior tree.

My original plan was to also do A* myself, but it turned out to take longer than I was expecting so I ended up using a library from: https://arongranberg.com/astar/ to complete the project.



3.	What game engine/tools/libraries will your game use?

I used the A* unity package from https://arongranberg.com/astar/ to do the pathfinding for the enemy AI.




4.	Why do you think your game is interesting/exciting? 

It is exciting based on the fast paced dodging and attacking. You need to kill enemies swarming at you and will need to dodge bullets in order to increase your score.


5. Other notes

I was the only member of my group so I did this project alone.