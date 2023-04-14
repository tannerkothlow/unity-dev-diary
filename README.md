# Unity 2D Dev Log and Guides

## Overview

This repo will serve as a way to document and share solutions I've found while working on a top-down RPG project in Unity.

Do note that this series of guides is a constant work in progress, so if some componants are incomplete, know they will be filled in relatively soon!

*View the most recent Dev Log Here: [Dev Log 1: The Two Month Mark](https://drive.google.com/file/d/1mjTNY5_GscEU3kTTi2KCqWWimnX81dzA/view?usp=sharing)*

## [Guides](./guides/)

This repo will contain a number of loose guides that broadly cover a number of objectives, such as how to simulate Z height in a 2D game, how to parse JSON objects as dialoge, and using prefabs for efficient workflow. These are not meant to be full comprehensive guides and instead highlight a use I have personally found for them. 

It is recommended that you have at least a basic understanding of code fundementals, familiarity with the C# script (Unity's primary coding language) and a fairly decent grasp on navigating the Unity Scene Editor. Likewise it is recommended to have a existing basic Unity project. [This tutorial from Brackeys is a good starting point](https://www.youtube.com/watch?v=whzomFgjT50), but no specific tutorial will be built off of in these guides.

Finally, assets referenced in the guides may be made availible in the accomponying `resources` folder, and will be hyperlinked for reference.

### [Top Down 3D Collision in 2D](./guides/top-down-3D-collision/)

What I mean by this is something along the lines of the *Mario and Luigi* series of RPG's where you traverse a 2D world in a top down view and stil have some form of simulated height. These guides will go over the general theory of what a platform *is* in terms of a game engine, and how we can apply that logic to a series of scripts that both control what collisions effect the player at a specified Z height, and sell the idea that we're truly moving in a 3D space by manipulating our player object.

Guides in `Top Down 3D Collision in 2D`:
- [Breaking Down The Problem](./guides/top-down-3D-collision/breaking-down-the-problem.md) 
- [Player Character](./guides/top-down-3D-collision/player-character.md) *Coming Soon!*
- [Adaptive Colliders](./guides/top-down-3D-collision/adaptive-colliders.md) *Coming Soon!*

### [Script Controlled Sprite Sorting](./guides/script-controlled-sprite-sorting/)

Despite Unity's fairly workable sprite systems, something that will always be frustratingly impersice is the baked in method of sorting single sprites tilemap chunks based on a loosely defined pivot point. With a script that's easy to both write and integrate, we can greatly improve the consistancy of our sprite organization.

Guides in `Script Controlled Sprite Sorting`:
- [Sprite Sorting](./guides/script-controlled-sprite-sorting/sprite-sorting.md) *Coming Soon!*

### [JSON Dialogue System](./guides/json-dialogue-system/)

For the purpose of a Unity dialogue system, you might need to store more data than just the to-be-rendered text. For instance, my project will have a number of text box shapes appropriate to the length of dialogue. Additionally, it's helpful to store animation data for the involved characters alongside the needed text. Therefor storing text in a JSON is a very efficient and readable way to store large amounts of dialogue, and with a few clever work arounds it's a surprisingly flexible method.

Guides in `JSON Dialogue System`:
- [NPC Interaction](./guides/json-dialogue-system/npc-interaction.md) *Coming Soon!*
- [JSON Parsing](./guides/json-dialogue-system//json-parsing.md) *Coming Soon!*
- [Embedding Special Insturctions](./guides/json-dialogue-system/embedding-special-instructions.md) *Coming Soon!*

### [Game Manager](./guides/game-manager/)

When transitioning between scenes in Unity, it wouldn't make sense to constantly despawn and respawn elements like the player character and HUD. Thanks in large part to the DontDestoryOnLoad method, persistant data across scenes is fairly simple to implement. Alongside a Game Manager object to hold methods for RPG battles, player state changes, and a HUD, you can truly begin to evolve from a tech demo to a crafted game world.

Guides in `Game Manager`:
- [Scene Persistance](./guides/game-manager/scene-persistance.md) *Coming Soon!*