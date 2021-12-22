# GB Studio 2.0 beta 5 Stair Climb Mod

A small modification to `Platform.c` implementing walkable stairs in platformer mode.


# How to Install

1. Eject the engine from your game.
2. Copy the file `Platform.c` from the folder `StairClimbMod/assets/engine/src/states/` in this mod to the same folder in your project.  For example: `YourGreatGame/assets/engine/src/states/`
3. Add stairs to the collisions in your game.


# How to Create Stairs

In this mod, stairs are represented by a combination of collision types.

| Type of Stair | Collision Combination |
| --- | ---|
| Climbed from the left | Collision Left & Ladder |
| Climbed from the right | Collision Right & Ladder |

When the engine sees these collision types placed together it interprets it as climbable stairs. 

**NOTE:** This means that the player cannot stand on top of these stair blocks.  Instead, a platform can be placed right below them.

Please check out the example project included here to see exactly how they work.


# Known Issues

1. Sometimes a player may pass through a climbable stair instead of climbing it.  This is unusual, but happens.
2. All climbable stairs are also ladders.
3. Climbable stairs cannot also be solid standing surfaces.


# Requirements

This game was built with [GB Studio 2.0-beta 5](https://github.com/chrismaltby/gb-studio/tree/v2beta#beta-builds).
I'm not sure if it will work with other versions.


# Contributors

- Code and sample project by [Paige Ashlynn](https://github.com/mxashlynn/).
- [GB Studio](https://gbstudio.dev/) is created by [Chris Maltby](https://github.com/chrismaltby/) and others.

# Rights

This mod may be used in your own games, including commercial and proprietary games.
See the `LICENSE` file for details.
