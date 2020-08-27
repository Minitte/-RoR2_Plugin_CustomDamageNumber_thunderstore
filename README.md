# Custom Damage Number Plugin

Allows you to change damage number's appearance:
- Texture
- Size
- Lifetime/duration
- Movement
- Toggle a custom material/shader to supports 11 digit damage numbers

Settings can be adjusted from the config file. (Risk of Rain 2/BepInEX/config/com.Minitte.CustomDamageNumbers.cfg)

## Installation
Extract the CustomDamageNumbersPlugin into /Risk of Rain 2/BepInEx/plugins/

## Making your own Damage Number Texture
- Use a square texture (512x512 is default)
- Split into 4x4 even sections (512x512 -> each section is 128x128 and there are 16 of them)
- Use the example damage number texture to know where numbers go
- Your custom texture goes into Risk of Rain 2/BepInEx/plugins/CustomDamageNumbersPlugin
- Configure the configs with the filename of your texture. (example: my_damage_texture.png)
- JPEG/.jpg does not support transparency!

You could also make one with google drawings using this template:
https://docs.google.com/drawings/d/19c3O1PdkXL4hDjM3GEcIc2-pJcNI7KgSr3U-0GCCW0I/edit?usp=sharing
1. File > Make a Copy
2. Open your copy of the template
3. View > Guides > Show guides
4. Use text box or drag in pictures or draw.
5. File > Download > PNG

## 11 Digit Damage Number Support
This uses a custom material/shader which is less stable and optimized than the default one. Kinda experimental.<br/>
Enabling this shader will override the default handling/format for spawning damage numbers. Other mods may not work with this enabled.<br/>
To enable: In config file, set useLongLineShader to true (useLongLineShader=true)

## Videos
More damage number digits: https://youtu.be/gWBg0716U44
Twitter animal emoji for damage: https://youtu.be/wcuTgsyHsAM

## Change Log
### 1.1.0
Added a custom shader option to support more damage number digits.

### 1.0.0
First released with features:
- Texture
- Size
- Lifetime/duration
- Movement

