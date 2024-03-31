## 👋 Hi there glad you found my Profile

My name is Fabio Mangiameli, I currently study computer science for media at the HdM in Stuttgart. I love game development and have a passion for programming.
Have a look at the projects I did during my studies.

Feel free to check out my [resume](https://drive.google.com/file/d/1_Em6ovbfWl9_z6pB7vfDodpsdytGMMDR/view?usp=sharing).

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

