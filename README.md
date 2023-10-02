## 👋 Hi there glad you found my Profile

My name is Fabio Mangiameli, I currently study computer science for media at the HdM in Stuttgart. I love game development and have a passion for programming.
Have a look at the game projects I did during my studies.

---

### Duskborn

Duskborn is a third-person shooter rouge-like. With a variety of movement options, you explore the world and upgrade yourself with items until you are powerful enough to beat the final boss. If you want to play the game you can download it for free on [Steam](https://store.steampowered.com/app/2474900/Duskborn/).

This game is the result of the game development lecture at HdM. It is supposed to be an experience as close to practice as possible. 18 people were developing the game split into different departments. My position was the Head of Engineering. Because the game was developed with Perforce I created a [Repository](https://github.com/MangiameliFabio/Duskborn) to showcase my code.

|<img src="/img/Duskborn_Boss.jpg"  width="387">|<img src="/img/Duskborn_Bottom_Abyss.png" width="387">
|---|---|
|<img src="/gif/Duskborn_WalkerFight.gif" width="387">|<img src="/gif/Duskborn_Grappling.gif" width="387">|

#### ⚙ Technologies I used
- Unreal Engine 5.1
- C++ and Blueprints
- Perforce
- Confluence
- Jira

#### 🗓️ Managing Tasks
- Leading a team of three people
- Organizing and conducting weekly meetings
- Creating tasks in Jira and distributing them to the team
- Managing the Perforce depot
- Creating tutorials on how to setup Unreal Engine and Perforce
- Collaborating with the other department heads to define milestone goals and discuss game features

#### 💻 Coding Tasks
- Implementation of player character logic
  -  State Machine for movement and combat behaviour
  -  Grappling hook mechanic
  -  Modular system for replaceable arm prostheses with different combat abilities
  -  Animation system for character body and each of the arm prostheses
- Developing an upgrade system
  - Crafting system
  - System to trigger item effects when the condition is fulfilled. Implementation was realized with the observer pattern.
  - Framework for the creation of item effects. The actual implementation of the specific effect could then be outsourced to the game design department.
- Implementation of the destructor enemy
- Created a system to distribute collectable loot through the level
- Enemy spawn system

---

### Curse of Immortality 

Curse of Immortality is a rogue-like dungeon crawler in which the player must face various challenges in an arena.  Most of the code I wrote you can find [here](https://github.com/Vel0X/CurseOfImmortality/tree/main/Source/CurseOfImmortality/AI). Feel free to also check out the rest of the source code and play the game.

|<img src="/img/Curse_of_Immortality_Combat.png" width="387">|<img src="/img/Curse_of_Immortality.png" width="387">|
|---|---|
|<img src="/gif/Curse_of_Immortality_Fight.gif" width="387">|<img src="/gif/Curse_of_Immortality_Boss.gif" width="387">|

#### ⚙ Technologies I used:
- Unreal Engine 5.0
- C++ and Blueprints
- Git
- Confluence

#### 💻 Tasks:
- Implementing enemy characters
  - Logic for six different enemy types each with different abilities and characteristics
  - Animation system for all enemies
  - General behaviour handled with state machine pattern
  - Implemented a heat map into our custom pathfinding
- Integrated arena traps into the damage system

---

### Crunch Time
Crunch Time was created during the [BeansJam 2022](https://itch.io/jam/beansjam-22). The theme for this game jam was "We have to stay awake" and we had 48 hours to develop it. Our game was rated place 7 out of 65 submissions!

The game is about a company late at night. You are the intern who needs to supply the workers with caffeinated drinks. Sometimes even the Sandman shows up and tries to put your coworkers to sleep. So you need to slap him out of existence. Check out our game on [itch.io](https://zwietabak.itch.io/crunch-time).

You can find the source code [here](https://github.com/MangiameliFabio/Crunch_Time).

|<img src="/img/Crunch_Time_Menu.PNG"  width="387">|<img src="/img/Crunch_Time_In_Game.PNG" width="387">|
|---|---|
|<img src="/gif/Crunch_Time.gif" width="387">|<img src="/gif/Crunch_Time_Zoomed_In.gif" width="387">|

#### ⚙️ Technologies I used:
- Godot 3
- GDScript
- Git

#### 💻 Tasks:
- Implementation of character logic
  -  Player character
  -  Sandman
-  Elevator mechanic
-  Sound implementation
-  UI implementation
   
#### State Machine Generator
For the character logic, I used a Godot plugin, which I created during the lecture Game Engine Programming to generate boilerplate code for state machines. The plugin will use template files to create Godot scripts. For more information have a look into the [repository](https://github.com/MangiameliFabio/State_Machine_Generator).

---

### Enchanted Defense
I wanted to learn more about the internals of a game engine and try out programming patterns. That's why I created this little game in a custom engine. I followed the [LazzyFoo SDL2 tutorial](https://lazyfoo.net/tutorials/SDL/index.php) to learn more about rendering with SDL2 and how to implement sounds. With the knowledge of the "Game Engine Programming" lecture from university and the book [Game Programming Patterns](https://www.amazon.de/Game-Programming-Patterns-Robert-Nystrom/dp/0990582906/ref=sr_1_4?__mk_de_DE=ÅMÅŽÕÑ&crid=3V71KG1U14PUB&keywords=Gameplay+programming+patterns&qid=1680433547&sprefix=gameplay+programming+patterns%2Caps%2C88&sr=8-4) I started coding. 

|<img src="/gif/Enchated_Defense.gif"  width="300">|<img src="/img/Enchanted_Defense_Menu.png"  width="300">|
|---|---|

#### ⚙️ Technologies I used:
- C++
- SDL 2
- Piskel
- Git

The global state of the engine is handled with a singleton. To update all my game objects I created an update loop in which all game objects can click in. For animations, I use sprite sheets. With the possibility of SDL2 to just render a specific part of an image I implemented a method to iterate through the different frames. A state machine is used to switch between different animations. I also created tools for measuring the performance of the engine internals and drawing debug shapes. <br>
For the Game, I use the command pattern in the input management to capsule input handling from the player character. With the observer pattern, I notify the game objects about stuff like the player dying or all inputs handled. To create enemies I used the prototype pattern. 

You can check out the project [here](https://github.com/MangiameliFabio/Top_Down_Shooter_in_custom_Engine).
