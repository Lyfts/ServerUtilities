# Ranks
Instead of giving each individual player permissions you can assign them ranks. You can give players can have multiple ranks in which case the rank with higher power takes priority.\

That mean if you have a rank like this
``` [player]
default_player_rank: true
power: 1
serverutilities.claims.max_chunks: 100
serverutilities.chunkloader.max_chunks: 50
serverutilities.homes.max: 1
```
and assign that same player to the admin rank as well the max homes will be 100 and the bypass limit permission will still apply.
```
[admin]
power: 100
serverutilities.claims.bypass_limits: true
serverutilities.homes.max: 100
```


### Commands

# Players


# Permission nodes

### Misc

| Permission node     | Description                                                                                                                                       | Available values |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|------------------|
| default_op_rank     | Default rank for OP and singleplayer with cheat enabled.                                                                                          | true/false       |
| default_player_rank | Default rank for players                                                                                                                          | true/false       |
| parent              | Determines the permissions to inherit from another rank                                                                                           | ""               |
| power               | Determines the power of a given rank. If a player is assigned multiple ranks <br/> the permissions from the one with highest power takes priority | 0-2147483646     |

### Claims
These permissions control what players can/can't interact with in claimed chunks as how many chunks can be claimed.

| Permission node                                      | Description                                                                    | Player Default | OP Default | Available values |
|------------------------------------------------------|--------------------------------------------------------------------------------|----------------|------------|------------------|
| `serverutilities.claims.attack_animals`              | Allow players to attack animals in claimed chunks                              | false          | true       | true/false       |
| `serverutilities.claims.block.edit.mod-id.block`     | Permission for blocks that players can break and place within claimed chunks   | false          | true       | true/false       |
| `serverutilities.claims.block.interact.mod-id.block` | Permission for blocks that players can right-click within claimed chunks       | false          | true       | true/false       |
| `serverutilities.claims.item.mod-id.item`            | Permission for items that players can right-click in air within claimed chunks | false          | true       | true/false       |
| `serverutilities.claims.bypass_limits`               | Allow to bypass claiming and loading limits                                    | false          | true       | true/false       |
| `serverutilities.claims.max_chunks`                  | Max chunk claims                                                               | 100            | 1000       | 0-30000          |


### Chunkloading

| Permission node                            | Description                                         | Player Default | OP Default | Available values |
|--------------------------------------------|-----------------------------------------------------|----------------|------------|------------------|
| `serverutilities.chunkloader.load_offline` | Keep loaded chunks working when player goes offline | true           | true       | true/false       |
| `serverutilities.chunkloader.max_chunks`   | Max Loadable Chunks                                 | 50             | 64         | true/false       |

### Chat Formatting

| Permission node                  | Description                                                                       | Player Default | OP Default | Available values                                                                                                                           |
|----------------------------------|-----------------------------------------------------------------------------------|----------------|------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| serverutilities.chat.formatting  | Allows to use **bold**, *italic* and ~~strikethrough~~ in chat                    | true           | true       | true                                                                                                                                       |
| serverutilities.chat.name_format | Format of the players name. Formatting codes goes inside the "<>" in the <{name}> | <{name}>       | <{name}>   | https://www.digminecraft.com/lists/color_list_pc.php                                                                                       |
| serverutilities.chat.text.color  | Color of the text when player sends a chat message                                | white          | white      | aqua, black, blue, dark_aqua, dark_blue, dark_gray, dark_green, dark_purple, dark_red, gold, gray, green, light_purple, red, white, yellow |

### Teleportation
| Permission node                 | Description                                         | Player Default | OP Default | Available values |
|---------------------------------|-----------------------------------------------------|----------------|------------|------------------|
| serverutilities.homes.cooldown  | /home Cooldown Timer                                | 5m             | 0s         | 0s to ∞          |
| serverutilities.homes.cross_dim | Can use /home to teleport to/from another dimension | true           | true       | true/false       |
| serverutilities.homes.max       | Max Homes                                           | 1              | 100        | 0-30000          |
| serverutilities.homes.warmup    | /home Warmup Timer                                  | 5s             | 0s         | 0s-1m            |
| serverutilities.rtp.cooldown    | /rtp Cooldown Timer                                 | 10m            | 0s         | 0s to ∞          |
| serverutilities.rtp.warmup      | /rtp Warmup Timer                                   | 5s             | 0s         | 0s to 1m         |
| serverutilities.spawn.cooldown  | /spawn Cooldown Timer                               | 1m             | 0s         | 0s to ∞          |
| serverutilities.spawn.warmup    | /spawn Warmup Timer                                 | 5s             | 0s         | 0s to 1m         |
| serverutilities.tpa.cooldown    | /tpa Cooldown Timer                                 | 3m             | 0s         | 0s to ∞          |
| serverutilities.tpa.cross_dim   | Can use /tpa to teleport to/from another dimension  | true           | true       | true, false      |
| serverutilities.tpa.warmup      | /tpa Warmup Timer                                   | 5s             | 0s         | 0s to 1m         |
| serverutilities.warps.cooldown  | /warp Cooldown Timer                                | 1m             | 0s         | 0s to ∞          |
| serverutilities.warps.warmup    | /warp Warmup Timer                                  | 5s             | 0s         | 0s to 1m         |                                                     |                |            |                  |               |

