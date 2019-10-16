# About
My personal configuration for the [Iris Keyboard](https://keeb.io/products/iris-keyboard-split-ergonomic-keyboard). The Iris is a pretty neat split keyboard that's based off of the [ergodox](https://www.ergodox.io/). I use it for my daily driver whenever I code. This repo mostly exists because sometimes I want to alter my workflow on the fly, but I do it so infrequently that I forget how to do it. Though if you want to use it or make alterations, go ahead!

For the full Cassandra expirence, try using my [Visual Studio Code theme](https://marketplace.visualstudio.com/items?itemName=Sitrusy.90s-anime) with it. It's an extra tacky semi-dark theme and I adore it.

[![xkcd comic](https://imgs.xkcd.com/comics/borrow_your_laptop.png)](https://xkcd.com/1806/)

## The Layout
- This layout is loosely based off of the [Lewis Ridden](https://github.com/qmk/qmk_firmware/tree/master/keyboards/keebio/iris/keymaps/lewisridden) configuration. Execpt for the weird parts. That's all me.
- I'm left handed, so the space is on the left thumb and enter is on the right. I'm aware this is not everyone's preference, so feel free to swap them.
- My config has the Raise and Lower levels on the upper parts of the thumb, so this requires a layout that has the thumb as two buttons.
- There's no caps lock. You've going to have to use your own charisma to be cool. Instead, Left Shift and Left Control is shifted up a key to make space for the Left Alt button on the left thumb row. The benefit is you can do any key combo with the left hand, provided it's around a letter on the left side.
- I optimized my layout for coding, so special characters like "_", '-' sit on the right thumb. At first, it was because I didn't know what to stick there and now I can't go back.

# How to Use
In order to use this keymap, you'll need to compile it first and flash it to the keyboard using QMK Toolbox. Don't forget that you need a recent version of [AVR build tools](https://docs.qmk.fm/#/getting_started_build_tools) installed if you decide to compile it on your own.
## Compiling
- Compile either using the command line in [QMK](https://docs.qmk.fm/#/?id=how-to-compile) (after adding the keymap folder, make: keebio/iris/rev2:cspruit)
- Preferred: use the online [QMK Configurator](https://config.qmk.fm/#/keebio/iris/rev2/LAYOUT) and import the keymap.json file and download the compiled .hex file

## Flashing
- Open the QMK Toolbox
- Add the compiled .hex file in the Local File section. Use the default atmega32u4 for Microcontroller.
- Check the "Flash when ready" box.
- Plug in the Iris keyboard (master half only if updating) and hit the physical reset switch to update keymap
- Test and make sure both halves work properly. I like using Switch Hitter by EliteKeyboards.com. The site's dead, but Switch Hitter lives on. [Major Geeks Mirror](https://www.majorgeeks.com/files/details/switch_hitter.html)
- If all works you should be good to go! If not, check over the [Keebio](https://docs.keeb.io/faq/) and [QMK](https://docs.qmk.fm) documentation to troubleshoot.
