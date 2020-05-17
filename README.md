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

### Overview

Unreal Engine: An application that is used to run games.

Unreal Editor: Application for creating games.

Level Editor: An editor inside of the Unreal editor.  This actually the default screen for the Unreal Editor.

Double clicking on assets in the editor will bring up the editor associated with that type of asset.  I.e. double clicking a material will open the material editor.

There are different components of the level editor in the default layout.
1. Viewport: used to give a visual representation of the game
2. Toolbar: Gives access to common functions
3. Content Browser: Storing and organizing
4. Modes Panel: Allows you to change the mode of the editor that make it easier to complete a discrete task.  I.e. 
5. World Outliner: Lists and groups the objects in the level
6. Details: View and edit parameters of the currently selected object

### Place Mode

Place Mode is used to place actors into your level.  Place mode is used for common generic actors, while the content browser is used to place custom actors.

To place an actor into your level, simply click on it in the Place Actors window and drag it into your level.  You can delete it by hitting the delete key while it is selected.

Place mode is grouped into different categories:

1. Recently Placed: Actors that you have used recently.
2. Basic: Basic actors
3. Lights: A light in the UE is a light projecting from a source. 
4. Cinematic: Tools to help create rendered 3D videos (cutscenes).
5. Visual Effects: Contain actors that add a variety of FX.
6. Geometry: Contain basic shapes.
7. Volumes: A 3D area of space that provide some functionality.  I.e. preventing a player from going somewhere.
8. All Classes: Contains EVERYTHING plus some that didn't fit into other tabs.

To quickly find a specific actor, you can type in the search bar at the top.

## Viewport Navigation

### Movement

The F11 key can be used to maximize the viewport on your screen.

Left clicking in the viewport allows you to rotate left or right and pan in the x and z direction.

Holding the left and right mouse buttons down or the middle mouse button down allow you to move in the y and z plane.

The right mouse button allows you to rotate the camera in any direction.

You can use the WASD keys while right clicking to move around in the viewport.  You can use the q and e keys to move up and down and the z and c keys to zoom in and out.  Zooming is only temporary though.

Clicking thee f key while an object is selected will focus the viewport on that object.

Holding the alt key while using the mouse will default to the viewport settings found in Autodesk Maya.

In the upper right section of the viewport, you can change the camera speed using the camera speed dropdown.

### Modifying Objects

There are different options in the upper right to move, rotate, or scale the currently selected object.  Shortcut keys are w, e, and r respectively.

You can move objects by dragging the area in the direction that you want to move.  You can also move in multiple axis by dragging the connector between them.  

You can select multiple actors by control clicking each one that you want to edit.

Holding down the shift key while moving an object will also move the camera with that object.

To make a copy of an actor, select it and hit ctrl + w or while using the move tool, his the alt key.  This also works with the rotate tool to create rotations of the same object.

World Space vs Local Space affect the axis and directions that objects will be edited in the world.  The scale tool will always be in world space.

### Snapping

The end key will allow you automatically snap an actor down to the nearest surface.

![Viewport Upper Right](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/ViewportUpperRight.PNG)

Surface snapping can be enabled with the surface snapping option in the upper right of the viewport. It only works when snapping in 3 dimensions.  Rotate to surface normal changes the rotation to match the surface normal.  While off it will maintain its rotation.  Surface offset tells the editor how far to put the actor to the surface of the object.

Grid snapping can be used to align objects across differences.  An incremental distance drop down can be modified to tell where to snap the object.  The snap unit is in cm.

Scale snapping functions similarly to the other incrementing options but in relation to scaling of objects.

### Level Viewing

The F11 key lets you toggle full screen mode in the editor (immersive mode).

The upper left options let you change different aspects of the level such as lighting.  I.e. Lit, Unlit, Wireframe.

![Viewport Upper Left](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/ViewportUpperLeft.PNG)

Specific orthographic views can be selected to view the level in a certain aspect.  i.e. top, left, right, etc.  When first selected they default to wireframe, but you can change it.

Show check boxes allow you hide certain objects in your viewport.  This is useful for hiding clutter while focusing on certain aspects of you level.

ctrl + shift + p allows you to pilot certain objects (such as lights) to get a first person view of what they can see.  This can be an easier placement method that transforming and rotating in your scene.

### Content Browser

The content browser gives you the ability to drag your own custom actors into the viewport.

![ContentBrowser](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/ContentBrowser.PNG)

The sources toggle button will toggle on/off a hierarchy of assets to help you navigate your project structure.  You can also search using the search bar.  Additionally, you can use the filters button to filter by file types or other parameters.  The top toolbar will show you the "breadcrumbs" that it took to get to that file.

You can add new assets into the content browser by using the "Add New" button in the upper left.

The import button lets you add your own content into the content browser.  Contents that are added to content browser are not saved until you click save all on the top toolbar.

In the bottom right you can change how your content is displayed in the content browser window.  i.e. tiles, list, folders, etc.

There are also different options to toggle on/off specific content such as in-development content, engine code, or plug-in code.

Collections let you group objects by parameters that you define.  I.e. a yellow chair could be added to a yellow collection and a chair collection.  Dynamic collections look for specific filters to add assets to.

You can navigate to the actor in the content browser while in the details window by clicking on the find button for that specific component.  You can also lock the window to make clicking find open a new window to that asset.

### Details Panel

The details panel gives you information about an actor that you currently have selected.  

![Details Panel](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/DetailsPanel.PNG)

At the top is the name of the actor.  There are also buttons for adding components and turning the currently selected actor into a blueprint.

The property matrix allows you to edit the value of multiple actors at once.

The transform component is common to all actors.  It provides you another way to modify actors in your level.  The yellow arrows to the right of the values will reset the values to a default.  You can change how the values are modified relative to the world or parent by selecting the dropdown on the property.  The mobility category allows you to change the type of the actor.

### World Outliner Panel

The world outliner panel is an organized list of all actors in the level.  

![World Outliner Panel](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/WorldOutlinerPanel.PNG)

The eye icon to the left of the actor allows you to toggle the visibility of it.  The icon will tell you what type of mobility the asset has as well as which category it is in.

You can drag actors onto other actors by dragging them onto other actors.  This means that when you move the parent it will move all the children.  Additionally, you can group actors by selecting and hitting ctrl + g.  Groups can be locked/unlocked to allow for individual editing of actors within a group.

## Actors

### Static Meshes

In UE there are static meshes and skeletal meshes.  Static meshes cannot move within the scene.  Skeletal meshes allow for actors with moving parts.

The static mesh component on an actor can be used to replace a mesh with another mesh.

By default, static meshes do not interact with physics.  To allow an object to interact with physics you need to set the mobility to movable and enable the simulate physics checkbox.

### Brushes

Brushes are used for creating basic geometry shapes.  Meshes only get stored in memory once whereas geometry brushes get stored 1 per geometry.  They are useful for prototyping and not meant to be used in the final product.

The hollow checkbox and options can be used to quickly create rooms and buildings.  Certain parameters will only be available if this option is selected.

### Materials

Materials are not actors, but are an important property of actors.  Materials give actors a texture and lighting characteristics.  Materials can be applied to brushes as well as meshes.

A single mesh may have multiple materials assigned to it.  Materials coordinates are labeled u and v.  When you scale an actor the material will also be scaled to fit the mesh.  

### Lights

In UE a ligth is an actor that generates a light in the level.  There are five types of light actors that you can use: 

1. Directional Light: Emulates ligth coming from a long distance away.  Primarily used for sunlight and moonlight.
2. Point Light: Produces light that emanates in all directions.
3. Spot Light: Generates ligth in the shape of a cone.
4. Rect Light: Projects lights in a plane.  I.e. tube lights, tvs, etc.
5. Sky Light: Represents light that is reflected (the faint glow of the atmosphere).

Changes in lights is not produced until being built in the editor.  This helps optimize performance in the editor.

Lights have several properties that can be modified including the mobility and transform.  Each type of light has additional unique parameters that can be adjusted.

![Light Properties](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/LightProperties.PNG)

### Atmospheric Fog

UE provides a few types of fog that can be added to your level: Atmospheric Fog and Exponential Height Fog.

An atmospheric fog actor makes the appearance of outdoor atmosphere.  This can be combined with a directional light to simulate actual sun location.  Atmospheric fog has additinal properties that you can modify.

![Atmosphere Properties](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/AtmosphereProperties.PNG)

### Player Start

The Player Start Actor defines where a player will start in your level.  If you want to test out starting from a different location, you can use the dropdown and select Play From Here.  Alternatively you can use the dropdown next to the Play Button and select Spawn Player at Current Camera Position.

### Components

Components allow you to change the properties of objects.  You can add new components through the Add Component button.  There is a convenient search functionality for searching by keywords.  When you add components in this way they are added as sub components that have their own unique properties.

Some components are only available as components and not as their own standalone actors, i.e. rotating an actor.

### Volumes

In UE, a volume is a 3D area of space and is invisible to the player.  They have some functionality tied to them such as damaging the player when they enter.  There are many volumes built-in to UE by default.

Trigger volumes are a highly useful volume that can be used to activate certain events when the player enters an area.

Pain Causing Volumes have the player take damage when they enter the volume.  Damage is a built-in construct for UE.

## Blueprints

### Blueprint Editor

Blueprints allow you to specify game logic such as tracking health, tracking game state, etc.

There are two main types:

1. Level Blueprints: Data and instructions for a particular level, i.e. time, keys, etc.
2. Blueprint Classes: A way to turn any Actor or asset into a blueprint (similar to prefabs in Unity)

Blueprint classes can be used to create as many copies (instances) that you want.  They are stored in the content browser.

You can open the level blueprint editor by selecting it in the top toolbar under Blueprints.

![Level Blueprint Editor](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/LevelBlueprintEditor.PNG)

The event graph that is in the center of the blueprint editor allows for visual scripting and also allows programmers to add C++ code.  It is a node based system where each node has a specific purpose.

The Event BeginPlay node is a node that occurs when gameplay begins.  The Event Tick node happens every "tick" of gameplay.

Function nodes are light blue and have a fancy f icon.  In blueprints, a function node is a node that performs a specific task.

![DelayFunctionNode](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/DelayFunctionNode.PNG)

Icons on the node are called pins.  Left side are called input pins and right side are called output pins.  Execution nodes denote the begin and end of the node.

### Variables

Variables can be used in UE to store data.  Variables can store numbers, text, etc.  They can be created in the Blueprint Editor by hitting the + sign under the Variables tab.

You can change the type of the variable by clicking the icon next to the name and selecting the type that you would like to use.

![VariableMenu](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/VariableMenu.PNG)

Once you create a get variable you need to compile the blueprint in order to be able to change the default value.  You can also create a set variable to set the value of a variable.  Once you set it, you can add it to the execution flow.

Tooltips can be added to the variables in order to provide a description of what that variable means.

Categories can be added to organize variables into groups.

Ranges can be added to keep a variable within a minimum or maximum range. 

### Arrays

Arrays let you store multiple values into one data type.  Any variable can be changed into an array by selecting the array option after clicking on the icon next to variable type.

![ArraySelection](https://github.com/masseydigital/unreal-beginner-tutorial/blob/master/imgs/ArraySelection.PNG)

Arrays have a variety of nodes that can be used to add, remove, insert, and modify values.  

### Functions

Functions are a specific procedure or routine meant to undertake the given task or series of tasks.  UE has functions in the form of node graphs.  Functions help provide reusable logic.

When a function is created, it starts with an entry node.  You can add inputs and outputs through the details pane.

The return node is the last node in the function and contains pins for each of your outputs.

### Flow control

Flow control is a set of nodes that help you control execution of your node graphs.  

A branch node takes in a boolean value and then executes code based on the input.  This is similar to an if statement.

Typing in "=" will show you all of the nodes that check for equality between two types including primitives like integers and also other more complex data types such as color.

The do n node will perform an action a number of times before blocking execution.  The do once node is similar but will only perform the action once before requiring the reset pin.

The flip flop node will flip between the a pin and b pin each time execution flows through the node.

The for loop node lets you choose your start and end index.

The gate node and multi-gate node allow you to specify conditions in which execution will travel through the gate.

The While loop gate will continuously perform an action when a given condition is true.

The switch node will follow a control based on the value of an input variable.

### Classes

You can create blueprint classes from actors that exist in your level.  A construction script is executed when your actor is created.

### Timelines

Timeline nodes help you create sequential animations.  They are a graph format where parameters are able to be modified over a given period of time.
