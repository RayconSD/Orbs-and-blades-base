The Concept 

Orbs and Blade is reken slash, top-down genre. The main idea is to move your character like in a MOBA, but perform special attacks like in a classic fighting game (such as Street Fighter). 
When you press an attack button, you need to move your mouse around your character to execute a special attack. For example, if you press "E" and move your mouse backwards and then drag it forward, your character will perform a lunge. 

Orbs and Blade Project Explained 

About the attack: 
<div>
  <img  align="center" alt="" Height="720" width="901" scr="https://cdn.discordapp.com/attachments/1233167310873956412/1358132038980337814/orbs__blades_-_GameMaker_05_02_2025_16_40_44.png?ex=67f2ba86&is=67f16906&hm=163812b58a6120625d8af9384be14471b0150bde4eacd5e497a1daf5cc5a5f3c&">
</div>

The first "if" activates some variables, like stopping the player movement, creating an array, taking the enemy's coordinates, and setting a timer for normal attacks. 

The second "if" is what triggers the attack. It uses an XOR because when the signal is sent to the weapon script, it considers whether the attack is low or heavy (E or R). But why XOR and not a normal OR? Because if E and R are used together, it will be a grab and not a normal attack. 

The switch is used to map the mouse's movement to determine which attack should be performed. 
