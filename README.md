# Why?

"But Tim, it's 2017, screensavers are unnecessary."

Hush you! I sleep better at night knowing that for 30 minutes ascii fish are
swimming around my screen before it blanks.

"Did you really write a Python GTK app to run a perl script in an embedded
terminal emulator?"

Yep.

# Prereqs

 * libcurses-perl
 * python-gtk2
 * python-vte
 * xscreensaver

# Installation instructions:

 1. Install prereqs

 ```
 # sudo apt-get install libcurses-perl python-gtk python-vte xscreensaver
 # cpan
 # cpan Term:Animation
 ```

 2. Install asciiquarium

 Assuming here that `~/bin` is in your $PATH

 ```
 # wget -O ~/bin/asciiquarium https://raw.githubusercontent.com/cmatsuoka/asciiquarium/master/asciiquarium
 # chmod +x ~/bin/asciiquarium
 ```

 3. Install the screensaver

 ```
 # cp asciiquariumxss ~/bin/asciiquariumxss
 # chmod +x ~/bin/asciiquariumxss
 ```

 4. Add `asciiquariumxss \n\` under `programs:` in `~/.xscreensaver`

 HINT: Make it the first screensaver in the list if it's not already.

 5. Test it out!

 ```
 # xscreensaver-command -select 1
 ```

# Credits

Made possible by stealing code from:

 * http://www.robobunny.com/projects/asciiquarium/html/
 * https://github.com/cmatsuoka/asciiquarium
 * http://alvinalexander.com/python/python-screensaver-xscreensaver-linux
 * http://nullege.com/codes/search/vte.Terminal
