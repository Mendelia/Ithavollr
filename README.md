# Iðavöllr
Minecraft private server organization repo :basecamp: __v1.21.4__  
This repository contains the files necessary to keep clients in sync, covering mods, resource packs, and config data. It also serves to link to all the other code repos that manage my [PaperMC](https://github.com/PaperMC/Paper) server instance.

## Directory
- [Content Manager](https://github.com/Ifiht/PacMan)
- [Data pack](https://github.com/Ifiht/Ithavollr-dpack)
- [Resource pack](https://github.com/Ifiht/Ithavollr-rpack)

## Packwiz Guide
### Setup
1. Import `com.unascribed.unsup.json` as a component in the Prism instance.
2. place `unsup.ini` in the `.minecraft` folder for the instance.
3. Run the instance.
### Update
1. `./packwiz refresh`
2. `./packwiz update --all`
### Update _Resource Pack_
1. Upload resource pack zip from PacMan actions to PacMan releases.
2. execute `./update_rpack.sh <URL>`, where URL is the link to the zip in the release.
3. remove the old toml file.
### Install new content
1. `./packwiz modrinth add <url>`

## TO-DO:
[ ] - Add back [RP-Renames](https://modrinth.com/mod/rp-renames) for 1.21.4 when available


## References
- Server
  + [Aincrad](https://github.com/Ifiht/Aincrad): WIP!! PaperMC fork aimed at adding new content/bug fixes.
- Tools
  + [unsup](https://git.sleeping.town/unascribed/unsup): Handles synchronization of all client environments.
  + [packwiz](https://packwiz.infra.link/tutorials/creating/adding-mods/): Organize and update client modifications. Syncs via unsup.
- Shader packs
  + [Complementary](https://modrinth.com/shader/complementary-reimagined): Best shader pack out there.
  + [Euphoria](https://modrinth.com/mod/euphoria-patches): Adds useful options to Complementary.
- Data packs
  + see [PacMan](https://github.com/Ifiht/PacMan): Merges all data packs into one monolithic pack for the server.
- Resource packs
  + see [PacMan](https://github.com/Ifiht/PacMan): Merges all resource packs into one monolithic pack for the client.
- Plugins
  + [Cardinal](https://github.com/Ifiht/Cardinal): Master plugin for Ithavollr. All other plugins are organized under its hierarchy.
