## Hi there glad you found my Profile👋

My name is Fabio Mangiameli, I currently study computer science for media at the HdM in Stuttgart. I love game development and have a passion for programming.
Have a look at the game projects I did during my studies.

---

### Duskborn

Duskborn is a third-person shooter rouge-like. With a variety of movement options, you explore the world and upgrade yourself with items until you are powerful enough to beat the final boss.

This game was developed as a project for the game "internship" at HdM. It is supposed to be an experience as close to practice as possible. We were 18 people developing the game split into different departments. I worked with Unreal Engine 5.1 and Perforce in this project.

|<img src="https://github.com/MangiameliFabio/MangiameliFabio/assets/92296151/ebe9356e-ec6f-40ea-be02-753bed54fde6"  width="500">|<img src="https://github.com/MangiameliFabio/MangiameliFabio/assets/92296151/a06f0949-6b99-49d6-b913-876279c2d460"  width="500">|
|---|---|
|<img src="https://github.com/MangiameliFabio/MangiameliFabio/assets/92296151/7cb9dec3-3c9b-4407-a8ca-19e1301016c4"  width="500">|<img src="https://github.com/MangiameliFabio/MangiameliFabio/assets/92296151/586caa04-bf45-4304-8ec0-461d03368c25"  width="500">

#### Technologies Used
- Unreal Engine 5.1
- Perforce
- Confluence
- Jira

#### Managing Tasks

I was head of engineering and led a small team of 3 people. I organized weekly meetings, created tasks and distributed them to the team. I was also responsible for setting up the project and managing a perforce repo. To make sure everyone is on the same page I created tutorials on how to install Perforce and Unreal. Especially important was the collaboration with the other heads. Together we defined new milestone goals and discussed new features for the game.


#### Coding Task

- Implementation of player character logic
  -  State Machine for movement and combat behavior
  -  Grappling hook mechanic
  -  Modular system for replacable arm prosthesises with different combat abilities
- Item system
  - Items cons


Besides managing, I was responsible for the implementation of the player character. The grappling hook mechanic was by far the hardest challenge. We needed a grappling hook which can pull the player towards the grappled point but also give the option of just hanging on the rope and swinging through the level. <br> 
To implement the behavior of the player character I used a state machine which can run two states at the same time. One state is the current movement state and the other one is the current combat state. In the future, the player should have the opportunity to change the prostheses of his character. Although the feature cant be seen in the game right now I implemented a system to make sure this is possible. 

Another task was the implementation of the upgrade system. I created a scheme which showed how the architecture should look and presented it to my colleague. Together we started the implementation. In the game, an item consists of two upgrade parts. One is the effect and the other one is the trigger. For example, an effect could be "spawn missile" and the trigger is "on kill" so the item will spawn a missile every time the player kills an enemy. To archive this I used the observer pattern for the triggers. For the effects, we wanted to have the possibility to create them in blueprints because game designer did the actual implementation of the effects. To craft an item during gameplay we used a factory. The factory will use two defined upgrade parts as input and generates the resulting item.

---

### Curse of Immortality 

Curse of Immortality is a rogue-like dungeon crawler in which the player must face various challenges in an arena. For this project, I worked with Unreal Engine 5.0 and Git. 

I was responsible for creating the enemy logic. To implement the character behavior I created a state machine component which is used on every character. In the game are 6 different types of enemies and all have different behaviour. Especially the final boss which can be seen in the second picture was a nice challenge because of the variety of attacks. We used custom pathfinding which was implemented by my colleague. Because the enemies tended to cluster in a group I implemented a heatmap into the pathfinding.

I also helped out with the traps in the arena and integrated them into our damage system.

I learned much about C++ and development in Unreal. Most of the code I wrote you can find [here](https://github.com/Vel0X/CurseOfImmortality/tree/main/Source/CurseOfImmortality/AI). Feel free to also check out the rest of the source code and play the game.

|<img src="https://github.com/MangiameliFabio/MangiameliFabio/assets/92296151/b5bfa58d-f5e6-40b8-b420-02ffd857194f" width="500">|<img src="https://user-images.githubusercontent.com/92296151/229345707-2f5b3a50-d35d-49c7-b642-3e5d39a6ffab.png"  width="500">|
|---|---|
|<img src="https://user-images.githubusercontent.com/92296151/229346938-0675cea1-288f-40cc-835c-7a00776dfe1b.png"  width="500">|

---

### Crunch Time
Crunch Time was created during the BeansJam 2022. The theme for this game jam was "We have to stay awake" and we had 48h to develop it. Our game was rated place 7 out of 65 submissions!

The game is about a company late at night. You are the intern who needs to supply the workers with caffeinated drinks. Sometimes even the Sandman shows up and tries to put your coworkers to sleep. So you need to slap him out of existence. Check out our game on [itch.io](https://zwietabak.itch.io/crunch-time).

You can find the source code [here](https://github.com/MangiameliFabio/Crunch_Time).

#### Technologies I used:
- Godot 3
- Git

#### Tasks:
-  Implementation of character logic
  -  Player Character
  -  Sandman
-  Elevator mechanic
-  Sound implementation
-  UI implementation

#### State Machine Generator
For the character logic used a Godot plugin, which I created during the lecture Game Engine Programming to generate boiler plate code for state machines. The plugin will use template files to create Godot scripts. For more information have a look into the [repository](https://github.com/MangiameliFabio/State_Machine_Generator).

|<img src="https://user-images.githubusercontent.com/92296151/229347667-b5bb6211-3296-40b1-a727-9a0710b97a4d.png"  width="300">|<img src="https://user-images.githubusercontent.com/92296151/229347778-0f0a5bb0-774c-4808-899a-75dc51fdf73b.png"  width="500">|
|---|---|
|<img src="https://user-images.githubusercontent.com/92296151/229347629-418eb8f5-c90a-4093-8187-5345a3c66849.png"  width="500">|
---

### Enchanted Defense
I wanted to learn more about the internals of a game engine and try out programming patterns. That's why I created this little game in a custom engine. I followed the [LazzyFoo SDL2 tutorial](https://lazyfoo.net/tutorials/SDL/index.php) to learn more about rendering with SDL2 and how to implement sounds. With the knowledge of the "Game Engine Programming" lecture from university and the book [Game Programming Patterns](https://www.amazon.de/Game-Programming-Patterns-Robert-Nystrom/dp/0990582906/ref=sr_1_4?__mk_de_DE=ÅMÅŽÕÑ&crid=3V71KG1U14PUB&keywords=Gameplay+programming+patterns&qid=1680433547&sprefix=gameplay+programming+patterns%2Caps%2C88&sr=8-4) I started coding. 

The global state of the engine is handled with a singleton. To update all my game objects I created an update loop in which all game objects can click in. For animations, I use sprite sheets. With the possibility of SDL2 to just render a specific part of an image I implemented a method to iterate through the different frames. A state machine is used to switch between diffrent animations. I also created tools for measuring performance of the engine internals and drawing debug shapes. <br>
For the Game, I use the command pattern in the input management to capsule input handling from the player character. With the observer pattern, I notify the game objects about stuff like the player dying or all inputs handled. To create enemies I used the prototype pattern. 

You can check out the project [here](https://github.com/MangiameliFabio/Top_Down_Shooter_in_custom_Engine).

For the gameplay, I was inspired by Stardew Valley's minigame that you play on one of the arcade machines. It is a top-down shooter in which you need to defend yourself against hordes of enemies. The Game is far from being finished. I intend to implement a UI, sounds, and custom data container to not rely on the standard C++ library anymore.

|<img src="https://user-images.githubusercontent.com/92296151/229348689-a0505f8f-a92a-4eff-9ed8-78ad2e8f3138.png"  width="300">|
|---|
