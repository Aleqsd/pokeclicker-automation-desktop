# Pokeclicker Desktop (With scripts support)

A web wrapper for Pokeclicker with scripts support

[![total downloads](https://img.shields.io/github/downloads/Farigh/pokeclicker-automation-desktop/total?label=total%20downloads&style=flat-square) ![downloads](https://img.shields.io/github/downloads/Farigh/pokeclicker-automation-desktop/latest/total?style=flat-square)](https://github.com/Farigh/pokeclicker-automation-desktop/releases/latest)

## Features from the [official Desktop App](https://github.com/RedSparr0w/Pokeclicker-desktop):
- Runs in background when minimised
- Works offline (after first run, once initial download completed)
- Auto download updates
- Discord rich presence (customizable)

![](https://i.imgur.com/5QQfoiZ.png)

## Features from the `With Scripts support` version:
- Runs the [pokeclicker-automation](https://github.com/Aleqsd/pokeclicker-automation), which can be disabled
- Allows to add more scripts to run (with toggles to enable/disable them individually)
- CLI support
```text
Available arguments:
  --help              Displays the help message
  --disable-scripts   Disables the custom scripts execution
                      This can be usefull if the scripts messes everything up
```

## Building
- `npm install` to pull Electron and builder dependencies.
- `npm start` to launch the app pointing at the Aleqsd automation fork.
- `npm run win` / `npm run win-portable` / `npm run linux` to create distributable builds.
- On first launch the app fetches the latest `master` snapshot of `Aleqsd/pokeclicker-automation` into your Electron user data folder; restart with `--disable-scripts` if you need to temporarily skip loading custom scripts.
