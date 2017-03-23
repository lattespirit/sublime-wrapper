# SublimeWrapper
**Sublime Wrapper** is a sublime plugin which can wrap selected content with specific code like `if`, `if/else`, `for`, etc. Supporting syntax includes `PHP`, `Python`, `Javascript`, `JSON`, highly inspired by PHPStorm's built-in surround feature.

![SublimeWrapper](http://i.imgur.com/JPk5P6m.gif)

# Installation

* ### Package Control(recommended)
    * To be continued

* ### Manual Installation
    * Using Git
        * Open terminal and change the path to Sublime `Packages` directory.(`Preferences > Browse Packages`).
        * Run `git clone https://github.com/lattespirit/SublimeWrapper.git`.
        * Done.

    * Using zip File
        * Click the `Preferences > Browse Packages…` menu.
        * Download the [Package](https://github.com/lattespirit/SublimeWrapper/archive/master.zip) file. Unzip and place the whole folder to the path methoned in Step One.
        * Rename the folder to `SublimeWrapper`.
        * Done.

# Configuration
* **SublimeWrapper** will map `"super/ctrl+k, super/ctrl+s"`(`"super"` means `Command` key in OSX) to trigger the command as default. If this key binding conflicts with the one in your environment, remap it to your favorite one without hesitation.
```json
[
    {
        "keys": ["super/ctrl+k", "super/ctrl+s"], "command": "activate_wrap"
    }
]
```

# Usage
* **Wrap Single Line:** Place the cursor in a single line, or select contents in the same line, then trigger the keymap metioned above, select the prefer item displayed in the popup panel, and press enter.
* **Wrap Multiple Lines:** Select contents in multiple lines, then trigger the keymap metioned above, select the prefer item displayed in the popup panel, and press enter.
    * **Notice: See Known Issuses below**
* **INFO:** When next_fields defined in the wrapper like **if/else**, press `tab` and jump to the next field. FYI, jumping to prev fields is NOT supported.

# Known Issues
 * When `Vintage Mode` is enabled and select a whole line or multiple lines in `Visual Mode`, trigger the key binding and wrap the selected contents. Then the whole view contents will be screwed up. Kind of nightmare.

# Contributing
* To be continued
