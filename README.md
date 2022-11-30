# Game Variables

Unity package library for sharing variable data across components and scenes.
Uses `ScriptableObjects` to store data and exposes events for when values change.

Heavily inspired by the infamous [Unite 2017: Game Architecture with Scriptable Objects](https://www.youtube.com/watch?v=raQ3iHhE_Kk) presentation by Ryan Hipple ([GitHub](https://github.com/roboryantron/Unite2017)).

## Installation

The package library can be installed to your Unity project one of two ways:

- Clone the repository and adding it as a local package
- Add the package by git URL

Installing it by git URL allows the package to be updated when new releases are available here.

## Documentation

See [Wiki](https://github.com/UnderLogic/game-variables/wiki/Variables) for documentation and usage.

## Samples

The package library includes several sample scenes that demonstrate how to use each type of variable component.
It is highly recommended that you import the samples so you can see the library in action and experiment with it.

## Contributing

To make working on the library easier while keeping this repository minimal, it is recommended to create a separate Unity project, (i.e. `game-variables-project`).

Then link the following folders into the Unity project for easy editing/syncing while keeping code completion and intellisense:

```shell
$ cd game-variables-project/Assets
$ ln -s ~/game-variables/Editor Scripts/Editor
$ ln -s ~/game-variables/Runtime Scripts/Runtime
$ ln -s ~/game-variables/Tests Scripts/Tests
$ ln -s ~/game-variables/Samples~ Samples
```

**NOTE:** This assumes both folders are in your `$HOME` folder. Adjust paths accordingly if they differ.

Now you can work in the shell project without copying files back and forth, and also generating `.meta` files automatically.
