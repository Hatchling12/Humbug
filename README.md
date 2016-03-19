Humbug
======

Minecraft server plug-in: Simply toggles various functionality

- Disables Anvil use.
- Disables Ender Chest use.
- Disables Villager trading.
- Disables Portal creation.
- Disables Ender dragon.
- Disables join/quit/kick announcements.
- Enables personal death message with coords
- Disables Death announcements.
- Enables Red coloring on Death announcements.
- Enables death message logging.
- Disables Enderman Griefing (stealing blocks)
- Enables Unlimited Cauldron Water
- Enables Quartz from Gravel
- Disables Wither block destruction radius.
- Disables Wither and Wither Skull explosions.
- Disables cobblestone generation from lava and water.
- Makes the Protection enchantment a little stronger
- Enables adjustment of all Player maximum health
- Fixes a rail duplication bug.
- Fixes a teleport bug when players log out while riding vehicles.
- Removes the Enchanted Book recipe.
- Removes the Enchanted Golden Apple recipe.
- Converts Enchanted Golden Apples to normal Golden Apples if a Player attempts to eat them.
- Disables Ender Pearl Teleportation
- Throttles Ender Pearl Teleportation
- Alters the downward acceleration of Ender Pearls
- Alters the drop rate of wither skulls
- Removes specific items from dropping when a mob is killed
- Prevents records from playing in jukeboxes
- Disabled dying sheep
- Disables water usage in main world hell biomes
- Prevents end portal tiles from being destroyed
- Prevents inventories, not your own, from being opened while in vehicles
- Prevents container carts from being opened
- Give projectiles a slow debuff on hit
- Multiplies mob death loot item count
- Disables experience except from XP bottles
- Finds End Portals in a world.
- Swaps Wither Skeletons or Ghasts in for Zombie Pigmen to raise their spawn rate.
- Adjust strength and health pots to pre-1.6 power levels
- Sets the base movement speed for all mounted horses
- Fixes a bug where players in destroyed minecarts fall through the block below
- Gives player saturation when they lose a point of hunger
- Prevents a bug that allows tree growth to wrap around the world and overwrite blocks at 1+.
- Adds option to (de)buff damage of arrows
- Adds options to sanitize signs on placement
- Adds option to sanitize existing signs in chunks

1.9 Feature Alterations:
- Disable Chorus Fruit teleportation
- Disable Elytra use

The 'humbug' console command can be used to get or set any of the configuration file settings while the server is running. Also available are 'humbug save' and 'humbug reload'.

Config file settings:
- debug: Boolean, Turns on debug logging (currently there is none)
- anvil: Boolean, Turns on anvil use
- ender_chest: Boolean, Turns on ender chest use
- ender_chests_placeable: Boolean, Allows ender chests to be placed
- ender_backpacks: Boolean, sets up Ender Chests as a backpack, dropped on quit/death/kick
- villager_trades: Boolean, Turns on villager trades
- portalcreate: Boolean, turns on portal creation
- enderdragon: Boolean, turns on ender dragon
- joinquitkick: Boolean, show part/quit and kick announcements
- deathpersonal: Boolean, send a private message to the person who dies, with coords
- deathannounce: Boolean, death message announcements
- deathred: Boolean, makes death announce messages red
- deathlog: Boolean, logs player deaths to the console
- endergrief: Boolean, turns on enderman stealing blocks
- unlimitedcauldron: Boolean, turns on unlimited cauldron water
- quartz_gravel_percentage: Integer between 0 and 100, 0 is standard behavior.
- wither: Boolean, Turns on the wither
- wither_explosions: Boolean, Turns on wither explosions destroying blocks. Wither/Wither Skull explosions will always occur to damage players, this only effects block breakage.
- wither_insta_break: Boolean, Turns on the wither insta-break ability
- cobble_from_lava: Boolean, Turns on cobblestone generation when lava and water mix
- cobble_from_lava_scan_radius: Integer, Sets the radius to scan for lava/water interaction
- ench_book_craftable: Boolean, Allows the Enchanted Book recipe to be used
- scale_protection_enchant: Boolean, Increases damage reduction granted by the Protection enchantment
- fix_rail_dup_bug: Boolean, Fixes a rail duplication bug
- fix_vehicle_logout_bug: Boolean, Fixes a teleport bug when players logout in vehicles
- player_max_health: Integer, sets all Player maximum health
- ender_pearl_teleportation: Boolean, Turns on Ender Pearl teleportation
- fix_teleport_glitch: Boolean, fixes glitchy Ender Pearl teleportation coords
- ender_pearl_teleportation_throttled: Boolean, Activates a cooldown between Ender Pearl teleports
- ender_pearl_gravity: Double, Alters the gravity which effects Ender Pearl -Y acceleration, default Minecraft value is 0.03
- ench_gold_app_edible: Boolean, Allows players to eat Enchanted Golden Apples. If false, Enchanted Golden Apples are converted to normal Golden Apples
- ench_gold_app_craftable: Boolean, Allows the Enchanted Golden Apple recipe to be used
- wither_skull_drop_rate: Integer between -1 and 1000000, -1 is standard behavior. If a random number [0, 1000000) is less then this value, a wither skull drops. For example, 200000 is a 20% drop rate.
- extra_wither_skele_spawn_rate: Integer between -1 and 1000000, -1 is standard behavior. If a random number [0, 1000000) is less then this value, a wither skeleton is spawned in the place of a zombie pigman. For example, 200000 is a 20% spawn rate.
- extra_ghast_spawn_rate: Integer between -1 and 1000000, -1 is standard behavior. If a random number [0, 1000000) is less then this value, a Ghast is spawned in the place of a zombie pigman. For example, 200000 is a 20% spawn rate.
- remove_mob_drops: List<Integer>, a list of item IDs to remove from the dropped items when mobs are killed. The in-game command can also accept Material names.
- disallow_record_playing: Boolean, Disables the ability for records to play in jukeboxes
- allow_dye_sheep: Boolean, defaults to true. Allows sheep to be dyed directly (rather than dyeing each bit of wool).
- allow_water_in_nether: Boolean, enables water use in hell biomes
- indestructible_end_portals: Boolean, makes end portal tiles indestructible
- prevent_vehicle_inventory_open: Boolean, prevent players in vehicles from opening inventories
- prevent_opening_container_carts: Boolean, prevent inventory minecarts from being opened
- projectile_slow_chance: Integer between 1 and 100 or out of bounds to disable, percentage chance of a projectile shot causing a slow debuff
- projectile_slow_ticks: Integer, number of server ticks a projectile shot's slow debuff will last
- loot_drop: Integer, multiplier to apply to mob death item counts
- ignore_experience: Boolean, disables BottleO (exp) controls
- disable_experience: Boolean, disables all vanilla experience but XP bottles
- xp_per_bottle: Integer, sets the amount of XP given to a player by an XP bottle
- find_end_portals: String, name of the world in which to search for end portals
- nerf_strength: Boolean, Nerfs the strength potion back to pre-1.5 mechanics
- buff_health_pots: Boolean, Buffs the health potion back to pre-1.5 mechanics
- horse_speed: Double, Sets the base movement speed of all mounted horses. This is MineCraft's adjustment ratio. The default 0.17 is just slower than a minecart.
- fix_minecart_reenter_bug: Boolean, Fixes the minecart re-enter bug where players in a destroyed minecart could fall through the world
- strength_multiplier: Integer, multiplier for added damage from strength potion levels.
- hunger_slowdown: Integer, amount of saturation to give a player when they lose a point of hunger
- saturation_multiplier: Double, adjusts saturation effect of food types, disabled if 0.0
- prevent_tree_wraparound: Boolean, prevents structure growth from wrapping around from the top of the world to bedrock causing block overwrite.
- disable_hopper_out_transfers: Boolean, disables transfers from hoppers to other hoppers or droppers
- bow_buff: Double, (de)buffs bow damage. Set to 1 for default, less than one for debuff, more than one for buff, 0 for no effect and less than 0 for heal.
- prevent_long_signs: Boolean, sanitize sign length
- prevent_long_signs_limit: Int, max individual sign text row length
- prevent_long_signs_allornothing: Boolean, if over limit clear line (if true) or truncate line (if false)
- prevent_long_signs_cancelevent: Boolean, if over limit just cancel the sign change event
- prevent_long_signs_in_chunks: Boolean, clears over-long signs from chunks as they load
- equipping_banners: Boolean, allows equipping a banner as a hat
- changing_spawners_with_eggs: Boolean, if True disables changing spawner type with a monster egg
- copy_book_enable: Boolean, if false disables book copying
- disable_bed_nether_end: Boolean, if true disables placing beds in the nether (specifically addresses exploding beds which appear to bypass Citadel)
- max_water_lava_timer: Integer, delay time to clearing lava/water propogation halt
- max_water_lava_height: Integer, height at which to control/eliminate water propagation
- max_water_lava_amount: Integer, number of water/lava blocks at which point further water propogation (over height limit) is halted
- obsidian_generator: Boolean, turns on 1.7-style obsidian generation mechanism
- drop_newbie_book: Boolean, enables welcome book dropping
- tag_on_join: Boolean, true enabled Combat Tagging on login (assuming Combat Tag is available)
- disable_entities_portal: Boolean, shortcut method to cancel all entity teleportation through portals
- disable_xp_orbs: Boolean, true to disable any XP drop from mobs 
- remove_pearl_chunks: Boolean, removes dropped Ender Pearls when a chunk unloads (ties into PrisonPearl)
- enchanting_table: Boolean, disables enchanting tables
- disk_space_shutdown: Double, percentage of disk space that, if less then this mark is available, triggers an orderly server shutdown
- disable_chorus_fruit: Boolean, disables teleportation using chorus fruit
- disable_elytra: Boolean, disables mounting or dismounting from elytra

Default configuration (biased for CivCraft):
- debug: false
- anvil: false
- ender_chest: false
- ender_chests_placeable: true
- ender_backpacks: false
- villager_trades: false
- portalcreate: true
- enderdragon: true
- joinquitkick: true
- deathpersonal: false
- deathannounce: true
- deathred: false
- deathlog: false
- endergrief: true
- unlimitedcauldron: false
- quartz_gravel_percentage: 0
- wither: true
- wither_explosions: false
- wither_insta_break: false
- cobble_from_lava: false
- cobble_from_lava_scan_radius: 0
- ench_book_craftable: false
- scale_protection_enchant: true
- fix_rail_dup_bug: true
- fix_vehicle_logout_bug: true
- player_max_health: 20
- ender_pearl_teleportation: true
- fix_teleport_glitch: true
- ender_pearl_teleportation_throttled: true
- ender_pearl_gravity: 0.06
- ench_gold_app_edible: false
- ench_gold_app_craftable: false
- wither_skull_drop_rate: -1
- extra_wither_skele_spawn_rate: -1
- extra_ghast_spawn_rate: -1
- remove_mob_drops:
- disallow_record_playing: true
- allow_dye_sheep: true
- allow_water_in_nether: false
- indestructible_end_portals: true
- prevent_vehicle_inventory_open: true
- prevent_opening_container_carts: true
- projectile_slow_chance: 30
- projectile_slow_ticks: 100
- loot_drop: 1
- ignore_experience: false
- disable_experience: true
- xp_per_bottle: 10
- find_end_portals:
- nerf_strength: true
- buff_health_pots: true
- horse_speed: 0.17
- fix_minecart_reenter_bug: true
- strength_multiplier: 3
- hunger_slowdown: 0.0
- saturation_multiplier: 0.0
- prevent_tree_wraparound: true
- disable_hopper_out_transfers: false
- bow_buff: 1.0
- prevent_long_signs: true
- prevent_long_signs_limit: 100
- prevent_long_signs_allornothing: true
- prevent_long_signs_cancelevent: false
- prevent_long_signs_in_chunks: true
- equipping_banners: true
- changing_spawners_with_eggs: true
- copy_book_enable: true
- disabled_bed_nether_end: true
- max_water_lava_timer: 1200
- max_water_lava_height: 100
- max_water_lava_amount: 400
- obsidian_generator: true
- drop_newbie_book: true
- tag_on_join: true
- disable_entities_portal: true 
- disable_xp_orbs: true
- remove_pearl_chunks: true
- enchanting_table: false
- disk_space_shutdown: 0.02
- disable_chorus_fruit: true
- disable_elytra: true

Defines a few utility commands:

/invsee <Player> to peak into an active player's main inventory.

/bahhumbug <Player> gives a player a holiday package

/introbook [<Player>] gives a player (or self) the intro-to-server book

/introkit [<Player>] OP command to give a player (or self) the intro kit

