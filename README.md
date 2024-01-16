# head_talking
A blender(4.0) plugin for reconstructing a human head from a single image, with the ability to input audio to drive speech.

## install

support blender 4.0.

1. download the [data.zip](https://drive.google.com/file/d/1vO0tpOS77OnG9SJXUe1EIY7LkRYA9l9p/view?usp=sharing), extract it into mh_admin. download the [data.bin](https://drive.google.com/file/d/1INX6exinaTuBinu3Pv5DYJJRdfRk8_Uc/view), put it into mh_anim(on my linux: `blender-4.0.2-linux-x64/4.0/scripts/addons/mh_anim`).

2. install the plugin, Edit->Preference->Install

3. search `mh_addon`, enable the plugin

4. install dependecies.
    copy `data/include` into blender's python include directory(result is: `.../4.0/python/include/python3.10/...`).
   
    for mac: `/Applications/Blender.app/Contents/Resources/4.0/python`
   
    for linux: `blender-4.0.2-linux-x64/4.0/python`
   
    for linux you need to install libopenblas-dev, `sudo apt install libopenblas-dev`
    ![](install_dependences.png)

## use the plugin

usage:

https://github.com/shengweiZHANG0/head_talking/assets/109774030/e43f29b3-8548-4728-8d69-003e91b53324

render result:

https://github.com/shengweiZHANG0/head_talking/assets/109774030/e836fd5b-0437-4c0b-a943-ef30e167f565
