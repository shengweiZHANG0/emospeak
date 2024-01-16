# head_talking
A blender(4.0) plugin for reconstructing a human head from a single image, with the ability to input audio to drive speech.

## install

support blender 4.0.
1. download the released zip package, put it into `blender***/scripts/addons/`.

2. download the [data.zip](https://drive.google.com/file/d/1SOXPyxppdtQqCbAgP9maew2lkVghh6na/view?usp=sharing), extract it into the plugin install dir - mh_admin. download the [data.bin](https://drive.google.com/file/d/1INX6exinaTuBinu3Pv5DYJJRdfRk8_Uc/view), put it into mh_anim(on my linux: `blender-4.0.2-linux-x64/4.0/scripts/addons/mh_anim`).

4. search `mh_addon`, `edit-> preference -> Add-ons`, enable the plugin
    ![enable_plugin](https://github.com/shengweiZHANG0/head_talking/assets/109774030/1be002e7-c357-46d3-acd7-e963524b6694)

5. install dependecies.
   Before installing the dependencies, you need to perform the following steps:
   * copy `data/include` into blender's python include directory.

        for mac the result should be: `/Applications/Blender.app/Contents/Resources/4.0/python/include/python3.10/[*.h]`
    
        for linux the result should be: `blender-4.0.2-linux-x64/4.0/python/include/python3.10/[*.h]`
    
        for windows the result should be: `blender-4.0.2-windows-x64/4.0/python/include/[*.h]`
        ![py_windows](https://github.com/shengweiZHANG0/head_talking/assets/109774030/085fe5a4-6480-498f-8082-bc87df0c7dd5)

   * copy `data/libs` into blender's python libs directory.

     only windows need todo so, the result should be: `blender-4.0.2-windows-x64/4.0/python/libs/[*.lib]`

   * install third libs

     for linux you need to install libopenblas-dev, `sudo apt install libopenblas-dev`
        ![](install_dependences.png)
   
## use the plugin

the first time it may need to download some model(.pth files), plese wait patiently.

usage:

https://github.com/shengweiZHANG0/head_talking/assets/109774030/e43f29b3-8548-4728-8d69-003e91b53324

render result:

https://github.com/shengweiZHANG0/head_talking/assets/109774030/e836fd5b-0437-4c0b-a943-ef30e167f565

## TOTO list

- [ ] skin texture reconstruction
- [ ] hair reconstruction
