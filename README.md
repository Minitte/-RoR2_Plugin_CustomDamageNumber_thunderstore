# Custom Damage Number Plugin

Allows you to change damage number's appearance:
- Texture
- Separate texture for critical hits
- Size
- Lifetime/duration
- Movement
- Max digits

Settings can be adjusted from the config file. (Risk of Rain 2/BepInEX/config/com.Minitte.CustomDamageNumbers.cfg) 
**@Minitte#6490** on the Risk of Rain 2 modding discord if you need something.

## Installation

### For r2modman 
- Just install with r2modman.

### For not r2modma
- Extract into the plugins folder 
- Should look kinda like this /Risk of Rain 2/BepInEx/plugins/Minitte-CustomDamageNumbers/

## Custom Texture Location
/Risk of Rain 2/BepInEx/plugins/Minitte-CustomDamageNumbers/
/Risk of Rain 2/r2modman/BepInEx/plugins/Minitte-CustomDamageNumbers/
Recommend backing up your own damage number texture/image file before updating.

## Making your own Damage Number Texture
- Use a square texture (512x512 is default)
- Split into 4x4 even sections (512x512 -> each section is 128x128 and there are 16 of them)
- Use the example damage number texture to know where numbers go
- Your custom texture goes into the plugin folder. (Risk of Rain 2/BepInEx/plugins/Minitte-CustomDamageNumbers/)
- Configure the configs with the filename of your texture. (example: my_damage_texture.png)
- JPEG/.jpg does not support transparency!

You could also make one with google drawings using this template:
https://docs.google.com/drawings/d/19c3O1PdkXL4hDjM3GEcIc2-pJcNI7KgSr3U-0GCCW0I/edit?usp=sharing
1. File > Make a Copy
2. Open your copy of the template
3. View > Guides > Show guides
4. Use text box or drag in pictures or draw.
5. File > Download > PNG

## 11 Digit Damage Number Shader (alternative)
This uses a custom material/shader which is less stable and optimized than the default one. **Kinda experimental.**<br/>
Enabling this shader will override the default handling/format for spawning damage numbers. Other mods may not work with this enabled.<br/>
To enable: In config file, set useLongLineShader to true (useLongLineShader=true)<br/>

Default(RoR2) shader vs the alternative:
- RoR2 dmg number shader squishes numbers together with more digits
- The alternative shader will only use the primary texture.

## Videos
More damage number digits: https://youtu.be/gWBg0716U44
Twitter animal emoji for damage: https://youtu.be/wcuTgsyHsAM
Math for damage (Separate critical hit texture): https://youtu.be/dY-SkWSEt2w

## Troubleshooting

### My damage numbers are white rectangles.
The path may not be correct. If you installed this manually, make sure the path to this plugin is:
Plugin Folder: /Risk of Rain 2/BepInEx/plugins/Minitte-CustomDamageNumbers/
Plugin DLL: /Risk of Rain 2/BepInEx/plugins/Minitte-CustomDamageNumbers/CustomDamageNumberPlugin.dll

## Change Log

### 1.2.2
- Updated installation instructions for non-r2modman players
- Added troubleshooting info for white rectangle issue
- Improved plugin path path processing

### 1.2.1
- Increased the default max digits to 6
- Fixed some typos on the readme

### 1.2.0
- Added options for a separate texture on critical hits
- Added more digit support using the default shader
- Included another sample damage number texture using math symbols

### Older change log entries in ChangeLog file.

