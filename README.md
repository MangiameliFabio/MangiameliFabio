## 👋 Hi there glad you found my Profile

My name is Fabio Mangiameli, I currently study computer science for media at the HdM in Stuttgart. I love game development and have a passion for programming.
Have a look at the projects I did during my studies.

Feel free to check out my [resume](https://drive.google.com/file/d/1SizebFSZdcD0t2-zH8UYJA-pzDX25AlE/view?usp=sharing).

---

### Enchanted Defense
I wanted to learn more about the internals of a game engine and try out programming patterns. That's why I created this little game in a custom engine. I followed the [LazzyFoo SDL2 tutorial](https://lazyfoo.net/tutorials/SDL/index.php) to learn more about rendering with SDL2 and how to implement sounds. With the knowledge of the "Game Engine Programming" lecture from university and the book [Game Programming Patterns](https://www.amazon.de/Game-Programming-Patterns-Robert-Nystrom/dp/0990582906/ref=sr_1_4?__mk_de_DE=ÅMÅŽÕÑ&crid=3V71KG1U14PUB&keywords=Gameplay+programming+patterns&qid=1680433547&sprefix=gameplay+programming+patterns%2Caps%2C88&sr=8-4) I started coding.

📂 Check out the [Source code](https://github.com/MangiameliFabio/Enchanted-Defense) <br>
🎮 Play the latest [Build](https://github.com/MangiameliFabio/Enchanted-Defense/releases/tag/Build) <br>
🎬 Watch the [Video walkthrough](https://drive.google.com/file/d/1DcSH0mLjfLbaEGVx8fJEFSZSX3N4aQHp/view?usp=drive_link) <br>

|<img src="/gif/Enchated_Defense.gif"  width="300">|<img src="/img/Enchanted_Defense_Menu.png"  width="300">|
|---|---|

#### ⚙️ Technologies I used:
- C++
- SDL 2
- Piskel
- Git

The global state of the engine is handled with a singleton. To update all my game objects I created an update loop in which all game objects can click in. For animations, I use sprite sheets. With the possibility of SDL2 to just render a specific part of an image I implemented a method to iterate through the different frames. A state machine is used to switch between different animations. I also created tools for measuring the performance of the engine internals and drawing debug shapes. <br>
For the Game, I use the command pattern in the input management to capsule input handling from the player character. With the observer pattern, I notify the game objects about stuff like the player dying or all inputs handled. To create enemies I used the prototype pattern.

---

### State Machine Generator

For the lecture Game Engine Programming, we got the task to create an addon for Godot. I love using state machines in my code but there's always plenty of boiler code to write. I created an addon which generates code for GDScript that you can completely modify. The plugin will use template files which include the code for a state machine.

You can see this addon in action in the source code of [Crunch Time](https://github.com/MangiameliFabio/Crunch_Time), a game which was created during the [BeansJam 2022](https://itch.io/jam/beansjam-22). Or look up the [repository](https://github.com/MangiameliFabio/State_Machine_Generator) to find out how to install and use it.

---

### Duskborn

Duskborn is a third-person shooter roguelite. With a variety of movement options, you explore the world and upgrade yourself with items until you are powerful enough to beat the final boss. If you want to play the game you can download it for free on [Steam](https://store.steampowered.com/app/2474900/Duskborn/).

This game is the result of the game development lecture at HdM. It is supposed to be an experience as close to practice as possible. 18 people were developing the game split into different departments. My position was the Head of Engineering. The development of Duskborn continued after the semester, but I was unable to take part due to my bachelor's thesis. For this project, an item system was created where items could be created from a trigger and an effect. I implemented and designed a tooling to make the development of the effects more accessible. This made it possible for game designers to participate in the development of the effects without needing in-depth knowledge of the code base.

📂 Because the game was developed with Perforce I created a [Repository](https://github.com/MangiameliFabio/Duskborn) to showcase my code <br>
🎮 Play the latest [Release](https://github.com/MangiameliFabio/Duskborn/releases/tag/Build) I was part of <br>
🎬 Watch the [Video walkthrough](https://drive.google.com/file/d/1FfdXbqWHlRajfGuDcEFj04kqFZ-m8qsq/view?usp=drive_link) <br>

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
  -  State Machine for movement and combat behavior
  -  Grappling hook mechanic
  -  Modular system for replaceable arm prostheses with different combat abilities
  -  Animation system for character body and each of the arm prostheses
- Developing an upgrade system
  - Crafting system
  - System to trigger item effects when the condition is fulfilled. Implementation was realized with the observer pattern.
  - Framework for the creation of item effects. The actual implementation of the specific effect could then be outsourced to the game design department.
- Implementation of the destructor enemy
- Created a system to distribute collectible loot through the level
- Enemy spawn system

---

## Game Jam Projects

### Crunch Time
Crunch Time was created during the [BeansJam 2022](https://itch.io/jam/beansjam-22). The theme for this game jam was "We have to stay awake" and we had 48 hours to develop it. Our game was rated place 7 out of 65 submissions!

The game is about a company late at night. You are the intern who needs to supply the workers with caffeinated drinks. Sometimes even the Sandman shows up and tries to put your coworkers to sleep. So you need to slap him out of existence. 

📂 Check out the [Source code](https://github.com/MangiameliFabio/Crunch_Time) <br>
🎮 Play the latest [Build](https://github.com/MangiameliFabio/Crunch_Time/releases/tag/Build) or play in the [Browser](https://zwietabak.itch.io/crunch-time) <br>
🎬 Watch the [Video walkthrough](https://drive.google.com/file/d/17bCTvuVgCx2NhOgqbx8xps5Kz3wg85nf/view?usp=drive_link) <br>

|<img src="/img/Crunch_Time_Menu.PNG"  width="387">|<img src="/img/Crunch_Time_In_Game.PNG" width="387">|
|---|---|
|<img src="/gif/Crunch_Time.gif" width="387">|<img src="/gif/Crunch_Time_Zoomed_In.gif" width="387">|

#### ⚙️ Technologies I used:
- Godot 3
- GDScript
- Git

#### 💻 Tasks
- Implementation of character logic
  -  Player character
  -  Sandman
-  Elevator mechanic
-  Sound implementation
-  UI implementation
   

---

### Scary Dark Dungeon
Scary Dark Dungeon was created during the [miniBeansjam 9](https://itch.io/jam/minibeansjam9). The theme for this game jam was "We are not alone" and we had 48 hours to develop it.

In Scary Dark Dungeon, you play John, a clueless farmer boy who fell through a hole into a dungeon. You now have to help him find his way out.

📂 Check out the [Source code](https://github.com/zwietabak/beansjam23) <br>
🎮 Play the latest [Build](https://fabiomangiameli.itch.io/scary-dark-dungeon) <br>
🎬 Watch the [Video walkthrough](https://drive.google.com/file/d/1U4cUO2n9wXgaAV6KUcL_lidTCazxMjWr/view?usp=drive_link) <br>

|<img src="/img/SSD_Screenshot_2.png"  width="387">|<img src="/img/SSD_Screenshot_4.png" width="387">|
|---|---|
|<img src="/gif/SDD_scene_1.gif" width="387">|<img src="/gif/SDD_scene_2.gif" width="387">|

#### ⚙️ Technologies I used:
- Godot 4
- GDScript
- Git
- Audacity

#### 💻 Tasks
-  Level and story design
-  Implementation of the dialogues
  - Using the plugin [dialoge nodes](https://godotengine.org/asset-library/asset/2214) as a framework
  - creating the dialogue sounds with an [animaliese generator](https://github.com/Acedio/animalese.js)
-  Sound implementation
-  Enemy character logic with my [state machine generator plugin](https://github.com/MangiameliFabio/State_Machine_Generator)
