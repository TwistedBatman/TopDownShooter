# Top Down Shooter



## Table of Contents
- [General Info](#General-Info)
- [Scenes](#Scenes)
  - [Main Menu](#MaiMenu)
  - [Credits Scene](#CreditsScene) 
  - [Game](#Game)
  - [Death Menu](#DeathMenu)
- [Main Scripts](#Main-Scripts)
  - [Enemy Objects](#Enemy-Objects)
  - [Item and Audio](#Item-and-Audio)
  - [Menus and Systems](#Menus-and-Systems)
  - [Player](#Player)
  - [Weapons and Grenades](#Weapons-and-Grenades)
  - [Object Spawner](#Object-Spawner)
  - [Screen Shake](#Screen-Shake)
  
## General Info

Top Down Shooter is a 2D game with top down view developed in Unity. The purpose of the game is for the player to survive for as long as they can. It’s an endless game with enemies spawning in waves. Each wave is more difficult than the previous and at certain waves a stronger enemy spawns (boss) and it’s required to be defeated in order to progress further. During the playthrough certain buffs appear that help the player. Every wave there is a chance for coins to spawn, the player can collect them and use them in the in-game store to purchase skins that change the character’s appearance.
Although it's a 2D game some elements like the player and the enemies are 3D objects.

## Scenes

There are 4 scenes in the game.

## MainMenu

It's the first scene that loads when the application is launched. It contains buttons with options to start the game (Play), enter the in-game store (Shop), open the Settings menu, watch the Credits, enter a code to redeem a one-time reward or exit the game.

![menu](https://github.com/TwistedBatman/TopDownShooter/assets/73825176/b3836912-7b91-4e09-9113-62374aa98c11)


**In-game store**

By playing the user can gather coins, they can then spend those coins in the shop to buy skins.
![shop](https://github.com/TwistedBatman/TopDownShooter/assets/73825176/1518fbb9-b507-48ca-a09f-9634b6e031b1)

**Settings Menu**

In the settings menu the user has different options to change the graphics and the volume.
![Settings](https://github.com/TwistedBatman/TopDownShooter/assets/73825176/4b6daa93-d28e-4a57-a493-17d7e0ccef4a)


## CreditsScene

It shows an animated text with credits.

## Game

The main scene where the user can play the game. The user can leave this scene either by pressing Escape (esc) and accessing a menu or if their character loses all its health therefore losing.



https://github.com/TwistedBatman/TopDownShooter/assets/73825176/aaa93faf-4047-4400-b162-fb4f1bc66188



## DeathMenu

This scene loads when the player loses by having their health reach 0. It gives the user the option to restart go back to the menu or exit the game. It also shows the current wave and score the player reached this round.

![end](https://github.com/TwistedBatman/TopDownShooter/assets/73825176/f605bd0e-7206-4f41-8fb4-67939b38da3a)


## Main Scripts

A quick explanation of each script by category.
#### Enemy Objects
- **EnemyController**: Exists in each enemy and controls them, by moving them to the direction of the player.
- **EnemyHealthManager:** Exists in each enemy and it contains their health.
- **HurtPlayer:** Exists in a game object within the enemy and it damages the player when they collide.

#### Item and Audio
- **AudioManager:** Controls the audio within the game.
- **Coins:** Manages the coins the player wins throughout the game.
- **DetectAndDestroyObjects:** Exists in each object spawned and it detects when the player collides with it in order to give them the corresponding buff.
- **ItemSpawner:** Spawns the corresponding item each time it’s called.
- **Sound:** Creates a slider the user can interact with to control the volume of the music.

#### Menus and Systems
- **Codes:** Implements a system where the user can enter a specific code and earn one-time rewards.
- **ExitCreditsScene:** Allows the player to leave from the credits scene when he presses Escape or after a specific time.
- **MainMenu:** Contains a variety of methods which are called from clicking buttons in order to change scenes.
- **PauseMenu:** It's called when the Escape button is pressed pausing the game and allowing the user to either leave or mute/unmute the volume.
- **SettingsMenu:** Provides the user with a variety of options to interact with, like changing the resolution or the volume.
- **WaveAndScore:** Show the score to the user and keeps track of the high score.

#### Player
- **HealthBar:** Visually shows and keeps track of the player health.
- **PlayerController:** Receives input from the user and controls the player character.
- **PlayerHealthManager:** Manages the player’s health removing or adding depending on the situation. It also gives a hit effect to the character by changing the color.
- **Skins:** Manages the in-game store by saving data on which skins the players has bought. It also allows the player to change the skin to one he has already bought.

#### Weapons and Grenades
- **BulletController:** Exists in each instance of the created bullets and it destroys the object when it hits an enemy or after a specific time.
- **GrenadeAmmo:** Visually shows how many grenades the player has.
- **GrenadeController:** Controls the time, damage and radius of the explosion.
- **GunController:** Controls when to fire or throw a grenade.

#### Object Spawner
- **Spawner:** It controls how many enemies to spawn per wave, when to spawn a boss and when to spawn items.

#### Screen Shake
There is also an imported asset from Unity Asset Store, containing 3 scripts, that controls the shaking of the camera.

