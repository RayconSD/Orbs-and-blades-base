The Concept 

Orbs and Blade is reken slash, top-down genre. The main idea is to move your character like in a MOBA, but perform special attacks like in a classic fighting game (such as Street Fighter). 
When you press an attack button, you need to move your mouse around your character to execute a special attack. For example, if you press "E" and move your mouse backwards and then drag it forward, your character will perform a lunge. 

Orbs and Blade Project Explained 

About the attack: 
<div>
  <img src="https://github.com/RayconSD/Orbs-and-blades-base/blob/main/orbs%20%26%20blades%20-%20triggers.png" alt="Texto alternativo" width="500" />
</div>

The first "if" activates some variables, like stopping the player movement, creating an array, taking the enemy's coordinates, and setting a timer for normal attacks. 

The second "if" is what triggers the attack. It uses an XOR because when the signal is sent to the weapon script, it considers whether the attack is low or heavy (E or R). But why XOR and not a normal OR? Because if E and R are used together, it will be a grab and not a normal attack. 

The switch is used to map the mouse's movement to determine which attack should be performed. 
