Mavis_Eos
=========

### About

This project was created to assist ETC Eos programmers with learning the positions of the keys on ETC Eos lighting desks (that helpfully keep moving between generations). I built this to build up my confidence - I prefer accuracy over speed when programming and have a habit of looking down to make sure I'm hitting the right keys in work environments. This was built to allow me to practice and build up my confidence that I'm right without looking at the keys in a low stress environment.

### Features
The software generates random Eos syntax, and displays them on a local webpage for the user to view and type into the Eos desk. When used with the included showfile, the syntax is sent back to the software to check your response, and if it is correct one point is added to the score. Five points are removed for any incorrect response.

## Installation

### Install Node Red
 1. Follow [this guide](https://nodered.org/docs/getting-started/local) on how to install Node Red for your system.
 2. Use the command `node-red` to start Node-Red.
 3. In the it will list the location on your computer of the settings file, `settings.js`. Find this file and open it in a text editor (like notepad).
 4. About 3/4 of the way down the document under Editor Settings, there should be a block that looks like this:
    ```        projects: {
            /** To enable the Projects feature, set this value to true */
            enabled: false,
            workflow: {
                /** Set the default projects workflow mode.
                 *  - manual - you must manually commit changes
                 *  - auto - changes are automatically committed
                 * This can be overridden per-user from the 'Git config'
                 * section of 'User Settings' within the editor
                 */
                mode: "manual"
            }
        },
    ```
    Change `enabled:false` to `enabled:true`, save and close the file.
5. Close the terminal running Node-Red, open a new terminal and run the `node-red` command again.
6. Navigate to http://localhost:1880
7. 