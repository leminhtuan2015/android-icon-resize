# Android Icons Generator

Generate different dimension of android icons and put it to proper folder.

** Install 

* python / python3
* pip

```sh
# Install pip
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py 
python3 get-pip.py
```

**Support dimensions:**

    xxxhdpi 192x192
     xxhdpi 144x144
      xhdpi 96x96
       hdpi 72x72
       mdpi 48x48

Usage
-----

    android_icons_generator.py <raw icon file> <res dir>/<prefix>
    
    `raw icon file` is the high resolution icon file.
    `res dir` is your Android project's res dir.
    `prefix` can be `drawable` or `mipmap`.

Examples
--------

    android_icons_generator.py ic_launcher.png ~/demoapp/app/src/main/res/mipmap
    android_icons_generator.py ic_person.png ~/demoapp/app/src/main/res/drawable
    
    python3 android_icons_generator.py ic_launcher.png ~/demoapp/app/src/main/res/mipmap
    python3 android_icons_generator.py ic_person.png ~/demoapp/app/src/main/res/drawable

A real example with execution result:

    $ android_icons_generator.py ic_launcher.png ~/awesome/app/src/main/res/mipmap 
    Generating ~/awesome/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png...
    Generating ~/awesome/app/src/main/res/mipmap-xxhdpi/ic_launcher.png...
    Generating ~/awesome/app/src/main/res/mipmap-xhdpi/ic_launcher.png...
    Generating ~/awesome/app/src/main/res/mipmap-hdpi/ic_launcher.png...
    Generating ~/awesome/app/src/main/res/mipmap-mdpi/ic_launcher.png...
    Done
