# Fallout Terminal Helper

Helper for Fallout Terminal Hacking Mini-Game.

## Overview

This Web-App can filter Passwords with the Likeness number. 

Steam Overlay Browser or a second PC might be an efficient method to use it. 

Javascript has to be enabled.

---
Since its complete client site, you can access it with GitHub pages: 

https://germanoid.github.io/terminal-helper/

---
Please note:

* You can only choose words with a chance to succeed. If you can't type a word, it's not the right one.
* The Programm doesn't restart automatically. If you found the word, just press ESC for a full reset.
* Tab = Autocomplete
* Enter = Send input
* Backspace = Delete last character

## Setup

To get an interactive development environment run:

    lein figwheel

and open your browser at [localhost:3449](http://localhost:3449/).
This will auto compile and send all changes to the browser without the
need to reload. After the compilation process is complete, you will
get a Browser Connected REPL. An easy way to try it is:

    (js/alert "Am I connected?")

and you should see an alert in the browser window.

To clean all compiled files:

    lein clean

To create a production build run:

    lein do clean, cljsbuild once min

And open your browser in `resources/public/index.html`. You will not
get live reloading, nor a REPL. 

## License

Copyright © 2014 FIXME

Distributed under the Eclipse Public License either version 1.0 or (at your option) any later version.
