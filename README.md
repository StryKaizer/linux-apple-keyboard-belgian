
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
