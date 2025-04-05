The Concept 

Orbs and Blade is reken slash, top-down genre. The main idea is to move your character like in a MOBA, but perform special attacks like in a classic fighting game (such as Street Fighter). 
When you press an attack button, you need to move your mouse around your character to execute a special attack. For example, if you press "E" and move your mouse backwards and then drag it forward, your character will perform a lunge. 

Orbs and Blade Project Explained 

About the attack: 
<div>
  <img src="https://github.com/RayconSD/Orbs-and-blades-base/blob/main/ob%20combo.gif" alt="Texto alternativo" width="500" />
</div>

The first "if" activates some variables, like stopping the player movement, creating an array, taking the enemy's coordinates, and setting a timer for normal attacks. 

The second "if" is what triggers the attack. It uses an XOR because when the signal is sent to the weapon script, it considers whether the attack is low or heavy (E or R). But why XOR and not a normal OR? Because if E and R are used together, it will be a grab and not a normal attack. 

<div>
  <img src="https://github.com/RayconSD/Orbs-and-blades-base/blob/main/orbs%20%26%20blades%20-%20array.png" alt="Texto alternativo" width="500" />
</div>

The switch is used to map the mouse's movement to determine which attack should be performed. 

In the obj weapon: 

  <img src="https://github.com/RayconSD/Orbs-and-blades-base/blob/main/orbs%20%26%20blades%20-%20triggers.png" alt="Texto alternativo" width="500" />

There are a bunch of "if" statements to read the array, compare it to the attacks of this weapon, and trigger the attack.

About the player animation: 

  <img src="https://github.com/RayconSD/Orbs-and-blades-base/blob/main/orbs%20%26%20blades%20-%20animacão.png" alt="Texto alternativo" width="500" />

I separated the player sprite into three parts (legs, head, and torso), because the weapon and player animations are different things. So when you attack, it doesn't matter how good the weapon animation is, your character just stands there... To improve the feeling of the attack, I made the character project himself in the direction of the attack. 
