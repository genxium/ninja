# Ninja vs EVILCORP

<img src="/assets/main-menu-1600x800.png" width="400"> <img src="/assets/gameplay-1-1600x800.png" width="400">

My entry for JS13K 2020.

**Ninja vs EVILCORP** is a platformer inspired by Super Meat Boy, Stealth Bastard Deluxe, and other great similar games.
The goal is to scale a tower to find the evil plans without getting spotted.

Levels were designed to offer obvious routes, as well as more difficult alternate routes, and a timer to allow speed running.

## Building
Please install [nodejs v11+](https://nodejs.org/en/) and [advancecomp v2.1](https://github.com/amadvance/advancecomp) to `$PATH` manually as prerequisites. To install `advancecomp` just decompress [this](https://github.com/amadvance/advancecomp/releases/tag/v2.1) and add it to `$PATH`.

```sh
make update
make build
```

## Testing

Test functionality is only available if you open `debug.html`.
You can then run commands in the browser's console.

### Time control

Press <kbd>F</kbd> to speed up the game, <kbd>G</kbd> to slow it down.

### Skip level

Press <kbd>N</kbd>.

### In-game level editor

A simple level editor allows you to modify the obstacles while in-game.

```javascript
setDebugValue('editor', true)
```

### Show grid

Press <kbd>T</kbd> while in game to show the grid.

### Set default level

```javascript
setDebugValue('level', levelIndex)
```

### Become invisible

```javascript
setDebugValue('invisible', true)
```
