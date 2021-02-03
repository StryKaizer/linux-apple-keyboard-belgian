# Belgian Apple azerty keyboard layout settings for linux

Fixes all keys I need when developing on a macbook pro running linux...
Also moves command and ctrl to behave similar to osx keybindings.


# Usage

Add new variant to evdev.xml

    sudo nano /usr/share/X11/xkb/rules/evdev.xml

    <variant>
      <configItem>
        <name>applemagic</name>
        <description>Belgian (Apple magic keyboard)</description>
      </configItem>
    </variant>
    <variant>
      <configItem>
        <name>macbookpro</name>
        <description>Belgian (Apple macbook pro)</description>
      </configItem>
    </variant>
        

Append bottom part from BE file (below commented line) to /usr/share/X11/xkb/symbols/be

    sudo nano /usr/share/X11/xkb/symbols/be

Or overwrite completely

    sudo cp -f be /usr/share/X11/xkb/symbols/.


## Note for development

Show pressed key code:

   xev

Search for keycode by finding matching code in /usr/share/X11/xkb/keycodes/evdev
