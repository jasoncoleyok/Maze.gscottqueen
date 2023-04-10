# Create a Maze
This exercise creates a small maze that aligns to the pro builder grid, the XR Origin component and its various components—in particular, the locomotion system (teleportation) and its associated providers as well as the XR Direct (grab)/Ray Interactors.

## Requirements

- The maze includes at least four turns.
The maze is simple and includes multiple turns on two levels.
![image showing dead ends](images/turns.png?raw=true "Turns")

- The maze includes at least two dead ends.
There are two dead ends that require the player to use a grabbable object to progress further.
![image showing dead ends](images/dead-end.png?raw=true "Dead Ends")

- The player must use a grabbable object to progress further.
![image showing dead ends](images/dead-end-door.png?raw=true "Dead End Door Requires Grabbable Object")
![image showing dead ends](images/grabbable-object.png?raw=true "Grabbable Object")

- A win state is activated upon entering the final section.
![image showing dead ends](images/win-state-inactive.png?raw=true "Win State Is Inactive")
![image showing dead ends](images/win-state-active.png?raw=true "Win State Is Active")

- The maze must be playable with the VR headset.
![image showing dead ends](images/vr-ready.png?raw=true "VR Ready")

## Challenges

There were many challenges to this exercise, but the most difficult was the creation of the maze itself. I had to create a maze that was both playable and visually appealing with the pro grid, and I had to do it in a way that was easy to understand and modify. I also had to make sure that the maze was playable with the VR headset.

To build the maze I used a unity asset that came with prototype ready prefabs. I then modified the prefabs to fit the grid.

The Teleport prefab includes the Teleporation Area component and a child object as a mesh collider. This made for easy placement of the teleportation area along with the Teleporation Reticle prefab for indicating where the player can teleport to.
