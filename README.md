***This project is unmaintained and was last tested on [this commit of OpenDream](https://github.com/OpenDreamProject/OpenDream/tree/1734412eb0b4ac577675f64fde9db4ba82a6c85a).***
# DMInRoblox
A proof of concept showing that OpenDream can be used to run DM in Roblox scripts.

## Getting Started
### Compiling DM
You must first compile the DM you want to run in Roblox. An example of such DM code can be found in the `DM/` folder.

First, you need to build the DMCompiler project. Refer to OpenDream's README for instructions on this.

Second, you must run the compiler on the DM code. To do this you run `DMCompiler.exe` with your DM file and `--nostandard` as arguments.

Finally, you must copy the resulting `.json` file into `src/server/DM.json`

### Building the Roblox Place
Building the Roblox place requires [Rojo](https://rojo.space).
To build the place from scratch, use:

```bash
rojo build -o "DMInRoblox.rbxlx"
```

Next, open `DMInRoblox.rbxlx` in Roblox Studio and start the Rojo server:

```bash
rojo serve
```

For more help, check out [the Rojo documentation](https://rojo.space/docs).