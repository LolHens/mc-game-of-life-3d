# Game of Life 3D (Minecraft Mod)
[![Build Workflow](https://github.com/LolHens/mc-game-of-life-3d/workflows/build/badge.svg)](https://github.com/LolHens/mc-game-of-life-3d/actions?query=workflow%3Abuild)
[![Release Notes](https://img.shields.io/github/release/LolHens/mc-game-of-life-3d.svg?maxAge=3600)](https://github.com/LolHens/mc-game-of-life-3d/releases/latest)
[![Apache License 2.0](https://img.shields.io/github/license/LolHens/mc-game-of-life-3d.svg?maxAge=3600)](https://www.apache.org/licenses/LICENSE-2.0)

[![](https://raw.githubusercontent.com/LolHens/mc-game-of-life-3d/master/fabric-1.16.2/src/main/resources/assets/gameoflife3d/icon.png)](https://www.curseforge.com/minecraft/mc-mods/game-of-life-3d)

This mod implements John Conway's Game of Life and a 3D variation by Carter Bays (variation 5766).
You can find out more about the variation here: https://wpmedia.wolfram.com/uploads/sites/13/2018/02/01-3-1.pdf

## Features
- Cell blocks that follow the rules of the Game of Life by John Conway (2333)
- Cell blocks that follow the rules of a Game of Life variation by Carter Bays (5766)
- Cell support blocks that can connect together separate cell structures to help you in activating them all at once

## Usage
- Place your cell blocks down in the desired structure.
- The cell blocks are still gray which means that the cells are not active yet.
- If you have multiple structures which are not directly connected but need to be activated together you can connect them using the cell support blocks. These blocks will disappear once you activate the structure.
- Right click one of the cell blocks or cell support blocks.
- The whole connected structure activates and the simulation starts.

## Requirements
### [Fabric](https://fabricmc.net/)
[<img src="https://fabricmc.net/assets/logo.png" width="32"> Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api)

[<img src="https://user-images.githubusercontent.com/1524059/88789314-e5dd3300-d196-11ea-99dc-2399393ef409.png" width="32"> Fabric Language Scala](https://www.curseforge.com/minecraft/mc-mods/fabric-language-scala)

### [Forge](https://files.minecraftforge.net/)
[<img src="https://avatars2.githubusercontent.com/u/1390178" width="32"> Minecraft Forge](https://files.minecraftforge.net/)

[<img src="https://user-images.githubusercontent.com/1524059/91673183-2849b500-eb33-11ea-8f9d-3d486f266000.png" width="32"> Scalable Cat's Force](https://www.curseforge.com/minecraft/mc-mods/scalable-cats-force)

[<img src="https://user-images.githubusercontent.com/1524059/94992271-30a96b80-0589-11eb-8fcd-b6c8ed66ad32.png" width="32"> MixinBootstrap](https://www.curseforge.com/minecraft/mc-mods/mixinbootstrap) (only required on 1.15.2)

## Recipes
#### Cell Support
![Cell Support](https://raw.githubusercontent.com/LolHens/mc-game-of-life-3d/master/screenshots/recipe_cell_support.png)
#### John Conway's 2D Cell
![John Conway's 2D Cell](https://raw.githubusercontent.com/LolHens/mc-game-of-life-3d/master/screenshots/recipe_cell_conway.png)
#### Carter Bays' 3D Cell
![Carter Bays' 3D Cell](https://raw.githubusercontent.com/LolHens/mc-game-of-life-3d/master/screenshots/recipe_cell_bays.png)

## Screenshots
![](https://raw.githubusercontent.com/LolHens/mc-game-of-life-3d/master/screenshots/2020-07-18_23.18.23.png)
![](https://raw.githubusercontent.com/LolHens/mc-game-of-life-3d/master/screenshots/2020-07-18%20232058.png)

## Videos
[![](https://img.youtube.com/vi/sQOsDWcU1sc/0.jpg)](https://www.youtube.com/watch?v=sQOsDWcU1sc)
[![](https://img.youtube.com/vi/5bM4YJ2GlI8/0.jpg)](https://www.youtube.com/watch?v=5bM4YJ2GlI8)

## Carter Bays' Game of Life 3D (5766)
The numbers 5766 define the game rules in this context:

- A cell requires a minimum of 5 neighbors to survive to the next generation.
- The cell can have at most 7 neighbors or else it dies of overpopulation.
- 66 means that a new cell is born if it has a minimum and maximum of 6 neighbors.

This is in contrast to the normal game rules 2333 by John Conway and allows the system to work properly in three dimensions. The lifeforms in 5766 should look very similar to the ones found in 2333. Another nice property of 5766 is that every 2333 structure works the same when it is 2 layers thick and sandwiched between two layers of other blocks. Here are a few examples of native 3D lifeforms:

[![](https://raw.githubusercontent.com/LolHens/mc-game-of-life-3d/master/screenshots/small_stable_life_forms_5766.png)](https://wpmedia.wolfram.com/uploads/sites/13/2018/02/01-3-1.pdf)

## Similar mods
There was already a Game of Life mod for fabric out there I didn't know about when starting to work on this mod so please check out [con-craft way life of game mine by TheEpicBlock](https://github.com/TheEpicBlock/concraftwaylifeofgamemine/)

## License
This project uses the Apache 2.0 License. See the file called LICENSE.
