# Create a Maze
This exercise creates a small maze that aligns to the pro builder grid, the XR Origin component and its various components—in particular, the locomotion system (teleportation) and its associated providers as well as the XR Direct (grab)/Ray Interactors.

## Walk-through
https://drive.google.com/file/d/1-ZKYlWDP6T0B8ZiOQU4k2r9F5hjYvbao/view?usp=sharing

## Requirements

- The maze is simple and includes multiple turns on two levels.
![image showing dead ends](images/turns.png?raw=true "Turns")

- There are two dead ends that require the player to use a grabbable object to progress further.
![image showing dead ends](images/dead-end.png?raw=true "Dead Ends")

- A win state is activated upon entering the final section, indicated by a red platform.
![image showing dead ends](images/win-state-inactive.png?raw=true "Win State Is Inactive")
![image showing dead ends](images/win-state-active.png?raw=true "Win State Is Active")

- The maze is VR headset ready.
![image showing dead ends](images/vr-ready.png?raw=true "VR Ready")

## Challenges

There were many challenges to this exercise, but the most difficult was implementing the interactions of grab and teleport mechanics. 

To build the maze I used a unity asset that came with prototype ready prefabs. I then modified the prefabs to fit and snap to the grid.

### Left Controller Rig == Teleport Locomotion
The Teleport prefab includes the Teleporation Area component and a child object as a mesh collider. This made for easy placement of the teleportation area along with the Teleporation Reticle prefab for indicating where the player can teleport to. Good use of the XR Ray indicator combined with the Line Renderer component to create a line that follows the player's controler aim.

### Right Controller Rig == Grab Interactor
The Grab Interactor prefab includes the XR Direct Interactor component. It uses a collider combined with an the XR Direct Interaction Layer to specify which objects can be grabbed.
