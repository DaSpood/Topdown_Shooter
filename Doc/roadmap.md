# Roadmap

Plan for the first (and most crucial) updates for the game. Updates have been split to regroup important key features, in an order that is judged to be pertinent for the development of the game. It is important that this order is strictly respected and that no features is added or removed from each update (though of course forgotten elements that belong within a feature should be added and documented).

All these updates are considered minor as they are pre-release updates. The last update will be a major release.

## Update 1: Project base

- Add map (world)
	- Fixed size: as big as the screen
    - Camera is immobile

- Add Player (player/mob)
    - Can move in all 8 directions without bug
    - Can collide with screen borders without going through

## Update 2: Camera and world interactions

- Change map (world)
	- Increase size
    - Camera centered around player, stopped by map borders (does not show outside the map)

- Add undestructible obstacles (world)
    - Player can collide with walls without going through
    - Player can go around walls without being stopped by 'invisible wall' hitbox

## Update 3: Weapon interactions

- Add Pistol (weapon)
    - ROF may be ignored
    - Can do damage
    - Hitscan works
    - Bullets can not hit multiple targets at once 

- Add Obstacle (weapon/prop)
    - No ammo depletion for now

## Update 4: Damages and upgrades

- Add Ennemy (mob/weapon)
    - Can be placed like an Obstacle
    - Can not move
    - Can not attack

- Add Score (system)
    - The score rewarded by a kill appears above the killed mob for a brief moment
    - The score rewarded takes into account the Score Multiplier

- Add Score Multiplier (system)
    - Can not decrease

- Add Upgrades (system)
    - ***From this point on it is implied that whenever a weapon is added, the corresponding upgrades are added as well***

## Update 5: Player-Mob interactions

- Update Mobs (mob)
    - Can now move with the correct pathfinding
    - Can now attack under the correct circumstances
    - Knockback upon hit works

- Update Player (player/mob)
    - Regenerates HP at a fixed rate
    - Can now die
        - Death is a Lose Condition 

- Add Lose Detection (system)
    - Triggered when a Lose Condition is met
    - For now, resets the game

## Update 6: Timers

- Update Weapons (weapon)
    - ROF now works correctly

- Update Mobs (mob)
    - ATK SPD now works correctly

- Update Score Multiplier (system)
    - Multiplier now decreases at a fixed rate

- Remove Zombie from weapon options (weapon)

- Add Infinite Wave (system)
    - Zombies will spawn at set locations on the map at a fixed rate

## Update 7: Explosives and Railgun

- Add Explosive Obstacle (weapon)
    - No ammo depletion for now
    - Explosions work correctly

- Add Lazer (weapon)
    - No ammo depletion for now
    - A hit does not stop the bullet

## Update 8: Menus

- Add Main Menu (menu)
    - Displayed in a dedicated area
    - Can select 'Play', which starts a new game sequence
    - Can select 'High Scores', which sends to the High Score Menu
    - Can select 'Quit', which closes the game

- Add High Score Menu (menu)
    - Displayed in a dedicated area
    - Can select 'Back', which sends to the Main Menu
    - Shows content of Score Saving file ordered by biggest to smallest

- Add Pause Menu (menu)
    - Displayed over current game sequence
    - Can be triggered using a key
    - Can be cancelled using the same key
    - Freezes the game but does not end it
    - Shows list of upgrades
        - Difference between obtained and locked upgrades

- Add Lose Menu (menu)
    - Displayed over current game sequence
    - Triggers the Score Saving
    - Can select 'Play Again', which starts a new game sequence
    - Can select 'Home', which sends to the Main Menu

- Add Score Saving (system)
    - Saves current score to a file
        - The score will be associated with a date

- Update Lose Detection (system)
    - Triggers the Lose Menu when triggered

## Update 9: Ammo and Loot Boxes --- Alpha release

- Add Loot Boxes (prop)
    - Spawns at set locations on the map at a fixed rate
    - Chance of refilling ammo or Player HP
        - Only able to give Player HP if the player does not currently have full HP
        - Only able to give ammo for unlocked weapons
        - Has equal chance to give ammo for all weapons available regardless of the current ammo count to ammo capacity ratio
        - When able to give Player HP, has 25% chance of giving Player HP. Ammo types are then equal within the remaining 75% chance

- Update Weapon (weapon)
    - Ammo depletion when firing now works correctly

- Update Player (player)
    - When the selected weapon runs out of ammo, the Player automatically switches to the Pistol
    - When a weapon is out of ammo, it can not be selected by the Player

***The project is now considered a playable game.***
