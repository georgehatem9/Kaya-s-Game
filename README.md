You are tasked with creating a game environment for an adventurous quest featuring a character named 
Kaya. Kaya must navigate through a beautifully designed terrain to find a magical staff that will activate 
moving platforms, allowing her to reach the top of a mountain where a sacred tree awaits. The game 
must be completed within a time limit of 360 seconds, or Kaya will face an unfortunate demise. 
Question 1: (20 points) 
Terrain Setup: 
• Use the provided heightmap and layers for terrain. 
• Rocky layer for elevations and mountains. 
• Grass layer for banks and roadsides. 
• Dirt/pebble layer for roads. 
• Place grass and mushrooms at your discretion. (You must put some grass and mushrooms)  
Atmospheric Effects: 
• Implement a natural-looking wind effect throughout the scene. 
• Create a raining effect using particle systems that covers a 100x100 area above Kaya. 
(Alternatively, a static rain fixed above the terrain can be used.) 
• Have a fog of 0.001 units. 
• All scene lighting must directly come from the provided skyboxes. 
Object Placement: 
• Put at least 500 trees, a mix of the two provided tree prefabs. 
• Position 3 rocks (provided assets) in designated spots (refer to the table at the end). 
Overlay texts: 
• Only a text showing Kaya’s remaining time is shown on the top at the middle of the screen. 
Kaya’s Movements: 
• Kaya is controlled using Unity's character controller with root motion. 
• Kaya has animations for Idle, Walk, Run, Jump Up, Air (Falling), Landing, Dying, and Idle 
Resting (Sitting).  
• Movement using 'W', 'A', 'S', and 'D', with Shift for sprinting. 
• Jumping with the space bar, with forward thrust based on the movement speed before the 
jump. (ranging from 2.0 to 4.0) 
Kaya's lost staff is placed near any of the 3 rocks, positioned 10 units in front (the rock is 
selected randomly at the beginning of each game). 
• Pick up the staff by pressing Left-Ctrl, only when in proximity, causing a red point light to 
shine. Kaya will be holding the staff in its right hand. 
Mini map: 
• Implement a mini map that can be toggled ON and OFF by pressing the ‘’M’ key. 
• The mini map should show a top view of the whole scene fixated above Kaya. 
• The mini map must be always moving with Kaya. 
• The mini map must be anchored to the top right of the screen and has a width and height equal 
to 25% of the whole viewport. 
Camera: 
• A freelook cinemachine must be following Kaya. 
• The details are provided in the table at the end.  
Question 2: (10 points) 
• Animations must be set as follows: 
o Root motion for ground movements. 
o Jumping is accomplished in three steps (Jump Up, Falling(Air), and Landing). 
o Kaya can fall off heights. In this case the falling animation should be played. 
o If no movements are detected, the idle animation should be playing. 
o If Kaya is walking, the walking animation must be played. 
o If Kaya is running, the running animation must be played. 
o As soon as Kaya picks the staff, the pick-up animation must be played, however, the 
staff is only picked at the appropriate animation time (When Kaya is crouching and 
grabbing it with its hands). 
o If Kaya wins, the sitting idle meditation animation must keep playing. 
o If Kaya dies, the dying animation will play once. 
• Implement A Way Finder Mechanism 
o If the player is pressing (and holding) the TAB key, a transparent bluish arrow should 
appear above Kaya’s head. 
o The arrow points Kaya to the exact location of the staff. (in front of any of the 3 
rocks). 
o As Kaya moves, the arrow must allows be pointing to where the staff is. 
o Use the provided asset for the arrow.
