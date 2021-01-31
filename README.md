# Usage

Add new variant to evdev.xml

    sudo nano /usr/share/X11/xkb/rules/evdev.xml

    <variant>
      <configItem>
        <name>applemagic</name>
        <description>Belgian (Apple magic keyboard)</description>
      </configItem>
    </variant>
        

Append last part from BE file to /usr/share/X11/xkb/symbols/be

    sudo nano /usr/share/X11/xkb/symbols/be

Or overwrite completely

    sudo cp -f be /usr/share/X11/xkb/symbols/.


## Note for development

Show pressed key code:

   xev

Search for keycode by finding matching code in /usr/share/X11/xkb/keycodes/evdev
   