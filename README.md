# Fusuma Configuration Features

  

This configuration file for Fusuma enables various touchpad gestures to control system functions on a KDE-based Linux system. Here's an overview of the available features:

  

## Rotate Gestures


### Three-Finger Rotation

- **Clockwise**: Increases screen brightness

	- Default: Increases by 10 units

	- With Right Ctrl or Left Ctrl: Increases by 5 units

	- With Left Shift: Increases by 50 units

- **Counterclockwise**: Decreases screen brightness

	- Default: Decreases by 10 units

	- With Right Ctrl or Left Ctrl: Decreases by 5 units

	- With Left Shift: Decreases by 50 units

  

### Four-Finger Rotation

- Both clockwise and counterclockwise rotations trigger the "Play/Pause" media key

  

## Swipe Gestures


### Three-Finger Swipe

- **Left**: Activates Alt+Tab (application switcher)

	- Subsequent swipes up, down, left or right move in the application switcher

- **Right**: Alt+Tab
  

### Four-Finger Swipe

- **Down**: Decreases system volume

- **Up**: Increases system volume

- **Right**: Mutes/unmutes speakers

- **Left**: Mutes/unmutes microphone

  
# Requirements

- [Fusuma](https://github.com/iberianpig/fusuma): Fusuma is required to recognize touch gestures
- [fusuma-plugin-keypress](https://github.com/iberianpig/fusuma-plugin-keypress): Fusuma plugin to recognize modifier keys
- [ydotool](https://github.com/ReimuNotMoe/ydotool): ydotool should be installed and run on startup, to emulate keypresses


# Configuration

- The config file should be placed in `~/.config/fusuma`
- The path for the key states file can be changed to your desired location

## Additional Notes


- The configuration uses `ydotool` for keyboard input simulation and `qdbus` for KDE-specific actions.

- Volume control is achieved through KDE's global shortcuts.

- A file at `~/projects/fusuma_key_states` is used to track the state of certain gestures.