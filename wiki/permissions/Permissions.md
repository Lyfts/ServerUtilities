# Permissions

## Claims
These permissions control what players can/can't interact with in claimed chunks as how many chunks can be claimed.

| Permission node                                      | Description                                                                    | Player Default | OP Default | Available values |
|------------------------------------------------------|--------------------------------------------------------------------------------|----------------|------------|------------------|
| `serverutilities.claims.attack_animals`              | Allow players to attack animals in claimed chunks                              | false          | true       | true/false       |
| `serverutilities.claims.block.edit.mod-id.block`     | Permission for blocks that players can break and place within claimed chunks   | false          | true       | true/false       |
| `serverutilities.claims.block.interact.mod-id.block` | Permission for blocks that players can right-click within claimed chunks       | false          | true       | true/false       |
| `serverutilities.claims.item.mod-id.item`            | Permission for items that players can right-click in air within claimed chunks | false          | true       | true/false       |
| `serverutilities.claims.bypass_limits`               | Allow to bypass claiming and loading limits                                    | false          | true       | true/false       |
| `serverutilities.claims.max_chunks`                  | Max chunk claims                                                               | 100            | 1000       | 0-30000          |
| Content Cell                                         | Content Cell                                                                   |                |            |                  |


## Chunkloading

| Permission node                                | Description                                         | Player Default | OP Default | Available values |
|------------------------------------------------|-----------------------------------------------------|----------------|------------|------------------|
| ```serverutilities.chunkloader.load_offline``` | Keep loaded chunks working when player goes offline | true           | true       | true/false       |
| `serverutilities.chunkloader.max_chunks`       | Max Loadable Chunks                                 | 50             | 64         | true/false       |
| Content Cell                                   | Content Cell                                        |                |            |                  |

| Permission node | Description  | Player Default | OP Default | Available values | |
|-----------------|--------------|----------------|------------|------------------|-|
| Content Cell    | Content Cell |                |            |                  | |
| Content Cell    | Content Cell |                |            |                  | |