# Bongo Cat Cam for Keyboard, Mouse & Mic

## About
A program that renders a scene that can be used as a fake cam.

The scene renders your relative mouse position, and displays a different hand when certain keys are pressed.

Intended to be used mainly for fullscreen games with many buttons.

## Usage
Currently only built a binary for Windows.

Download the most recent release, unzip, and run 'bongocat.exe'

Will remember window position.

In OBS: Add Window Capture -> Right Click the Window Capture -> Filters -> Add Chroma Key -> Key Color Type: Green

Press Ctrl+Shift+O to change settings.
###### Settings
* Resolution Width: Your monitor's resolution width
* Resolution Height: Your monitor's resolution height
* Border: Whether or not to draw a border on the bottom left, bottom, and bottom right areas.
* Microphone: Whether to animate mouth based on microphone volume.
* Left, Right, Forward, Back & Wave Keys: Comma Separated Numbers that refer to the keycodes of keys ([keycodes](https://keycode.info/))
  * Left/Right/Forward/Back/Wave refers to which image will be drawn when pressing a key in that list

Resolution Width/Height can be changed to be bigger/smaller to support multiple monitors.

App Config File: `C:\Users\<User>\AppData\Roaming\bongocat\config.json`

Window Config File: `C:\Users\<User>\AppData\Roaming\bongocat\window-state.json`

## Dev

#### Setup
`git clone https://github.com/Barkuto/bongocat.git`

`cd bongocat`

`npm install`

Set `dev = true` in `main.js` to make dev tool consoles appear in the windows.

#### Commands
* npm start : Runs app
* npm run dist : Builds a binary for the current OS

## Notes
* Based off of https://github.com/kuroni/bongocat-osu
* Credits to [kuvster](https://github.com/Kuvster) for his work on the arm curve function.
* The keyboard, mouse, and mousepad are the ones that I use :>
* Images can be changed inside the resources/app/img/ folder. Keep the images the same size, otherwise they will not work properly.
* Windowed games can be supported, if enough people need it to be so.