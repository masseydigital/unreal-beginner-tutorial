# unreal-beginner-tutorial
Learning the beginnings of Unreal...

## Introduction

### Sections

1. Getting Started
2. Level Editor
3. Actors
4. Blueprints
5. Players and Input
6. Collisions
7. User Interfaces
8. Audio
9. Additional Topics

### Installation

Download Launcher Link: https://www.unrealengine.com/en-US/

### Projects

Each game that you create will be stored in a project.  There is a browser in the launcher that shows your projects.  Projects are only loaded into the launcher if they have been opened in UE before.

There are (4) defaults that you can use to get started creating in UE4.
1. Games
2. Film, Television, and Live Events
3. Architecture, Engineering, and Construction
4. Automative, Product Design, and Manufacturing

![Project Settings](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/Project%20Settings%20Screen.PNG)]

After selecting the type, you can further select which kind of game you would like to create based on several other templates.

![Templates](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/Project%20Template%20Screen.PNG)

Once you select if you would like to use a template, the next page will allow you to select even more different options such as:

1. Blueprints vs. C++
2. Quality
3. Raytracing
4. Target Platform
5. Start Content

![Project Types](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/Project%20Type%20Screen.PNG)

When you create a new project, it should look like the following:

![Editor](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/UE%20Editor%20Example.PNG)

### Levels

_Definition:_ A collection of objects and their properties that together define their area of gameplay.

A single game will consist of many many levels.

In UE, you can create a new level by going to File > New Level.  This will bring up the new level screen which contains options for different defaults you can use.

![Editor](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/LevelDefaultSelector.PNG)

UE contains assets which are basically anything that is used to develop your game.

### Actors

Definition: An actor is any object that can be added to the level.  They can be physical objects in your level or other objects that define different components of your game.

_Static meshes_ refer to meshes with no moving parts.

_Geometry Brushes (or just Brush) are actors represented in 3D space.  Brushes are only meant to be basic 3D shapes vs. Meshes which can be complex.  Brushes are generally not as performant as meshes.  They are used to prototype levels.

UE has materials which make an object look like it has certain texture and lighting characteristics.

## Level Editor