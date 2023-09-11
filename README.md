# 2D Top Down Shooter

## General Info

Top Down Shooter is a 2D game with top down view developed in Unity. The purpose of the game is for the player to survive for as long as they can. It’s an endless game with enemies spawning in waves. Each wave is more difficult than the previous and at certain waves a stronger enemy spawns (boss) and it’s required to be defeated in order to progress further. During the playthrough certain buffs appear that help the player. Every wave there is a chance for coins to spawn, the player can collect them and use them in the in-game store to purchase skins that change the character’s appearance.
Although it's a 2D game some elements like the player and the enemies are 3D objects.

**Table of Contents**
- [Scenes](#Scenes)
 - [Main Menu](#MaiMenu)
 - [Credits Scene](#CreditsScene) 
 - [Game](#Game)
 - [Death Menu](#DeathMenu)
- [Main Scripts](#Main Scripts)
 - [Enemy Objects](#Enemy Objects)
 - [Item and Audio](#Item and Audio)
 - [Menus and Systems](#Menus and Systems)
 - [Player](#Player)
 - [Weapons and Grenades](#Weapons and Grenades)
 - [Object Spawner](#Object Spawner)
 - [Screen Shake](#)

## Scenes

There are 4 scenes in the game.
#### MainMenu
It's the first scene that loads when the application is launched. It contains buttons with options to start the game (Play), enter the in-game store (Shop), open the Settings menu, watch the Credits, enter a code to redeem a one-time reward or exit the game.
ΕΙΚΟΝΑ
**In-game store**
By playing the user can gather coins, they can then spend those coins in the shop to buy skins.
ΕΙΚΟΝΑ
**Settings Menu**
In the settings menu the user has different options to change the graphics and the volume.
ΕΙΚΟΝΑ

#### CreditsScene
It shows an animated text with credits.
Game: The main scene where the user can play the game. The user can leave this scene either by pressing Escape (esc) and accessing a menu or if their character loses all its health therefore losing.
ΒΙΝΤΕΟ

#### DeathMenu
This scene loads when the player loses by having their health reach 0. It gives the user the option to restart go back to the menu or exit the game. It also shows the current wave and score the player reached this round.
ΕΙΚΟΝΑ

## Main Scripts

#### Enemy Objects
- **EnemyController**: Exists in each enemy and controls them, by moving them to the direction of the player.
- **EnemyHealthManager:** Exists in each enemy and it contains their health.
- **HurtPlayer:** Exists in a game object within the enemy and it damages the player when they collide.

#### Item and Audio

#### Menus and Systems

#### Player

#### Weapons and Grenades

#### Object Spawner

#### Screen Shake

