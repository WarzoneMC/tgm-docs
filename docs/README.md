## Warzone
> ### Welcome to the TGM Maps Documentation Site!

This website is for documenting implementations of [WarzoneMC's Fork](https://github.com/WarzoneMC/Warzone) that is used live on [warzone.network](https://warzone.network).

### What is TGM?

TGM is a team-oriented Minecraft PvP suite inspired by [PGM](https://github.com/OvercastNetwork/ProjectAres). TGM's goal is to shift most of the game logic to Java, which allows for rapid development and modernization of gamemodes over time. TGM parses something called JSON (JavaScript Object Notation) in order to load and manage maps on the server, which are handled by the server's [rotations](https://github.com/WarzoneMC/Maps/blob/master/rotation.txt). The development of TGM is primarily driven by the community.

### What do JSON files do?

JSON files allow the server to communicate exactly how matches should operate. JSON defines aspects of the game such as filters, teams, kits, regions and more. Each file is unique to its map, however the components and modules are generic and are used across several different maps. These are required in order for the map to load on the server.

### How do I write JSON files?

JSON files can be written in any text editing program, however the most efficient way is to use a program that can automatically indent and syntax your code. Programs like [Atom](https://atom.io/) and [Notepad++](https://notepad-plus-plus.org/) are commonly used for these standards. Files must use modules available on this documentation site.

### How do I test my JSON files?

JSON files must be fully functional in order to be loaded onto a TGM server without errors. To test your JSON, you may create a local server running TGM. If you wish to test whether or not your JSON will parse, you may use [jsonformatter.org](https://jsonformatter.org/json-parser).

1. Start with the latest stable [Paper (PaperSpigot)](https://papermc.io/ci/job/Paper/) build. 
 
2. Create a `Maps` folder inside of the server and insert the TGM map with your `map.json`, `region`, and `level.dat` files.

3. Start the server.

---

Feel free to contribute to the development of this website by [making pull requests on GitHub!](https://github.com/WarzoneMC/Docs/) This website is community maintained.


