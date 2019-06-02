# GameHook

This is a fork of [the refactor branch](https://github.com/philkr/gamehook/tree/refactor) of [GameHook](https://github.com/philkr/gamehook).

IMPORTANT: Before doing anything, please read the [instructions in the original README](https://github.com/philkr/gamehook).

The refactor branch adds support for per-pixel texture ids,  
and this fork allows the python plugin to access all targets (disparity, flow, ...).

## Installation

This project requires Microsoft Visual Studio,  
build `gamehook.sln` in the `Release x64` configuration.  

You might have to fight some linking issues -  
This will require going into a submodule's `Properties > C/C++ > General` page,  
and mangling the `Additional Include Directories`.

After a successful compilation, transfer the following files into the target game's directory.

```
python.hk
server.hk
gamehook.dll -> manually rename this to -> dxgi.dll
```
