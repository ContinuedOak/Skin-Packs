# Custom Skin-Packs

## Getting Starting
Before you start you'll need to make sure you have everything installed correctly.

Firstly make sure you have [Legacy Skins](https://modrinth.com/mod/legacy-skins), [Legacy 4J](https://modrinth.com/mod/legacy4j) and [Customizable Player Models]([https://modrinth.com/mod/legacy4j](https://modrinth.com/plugin/custom-player-models).

Once all are installed you can now follow these steps:

# How to Make a pack
### Step 1
Load into world and press (G) by default to open the Customizable Player Model Editor, go to models and click "Open Skin Editor".

### Step 2
Create and/or load the skin/model you want.

### Step 3
When ready to export, go to file - export, upon viewing the export screen, change 'Export Mode' to 'Model'.

### Step 4
Rename it to the name of the model, keep it simple and IT MUST STAY IN LOWERCASE AND NO SPACES (ie: defaultsteve).

### Step 5
Then press export. the file will now be saved to 'player_models' folder inside your instances.

### Step 6
Create a new folder inside your 'resource_pack' folder (ie: 'ExampleSkinPack')

### Step 6
Inside this pack recreate a regular resource pack with a pack.png, pack.mcmeta and a folder called assets. To learn more about pack.mcmeta and what format to use head to the [minecraft-wiki](https://minecraft.wiki/w/Pack_format).

### Step 7
Now onto the Skin Pack itself. Inside the assets folder create a new folder, this can be the same as the title but it is used to simplify creating multiple skin packs so if you are creating.

### Step 8
Inside the previously made skin pack folder, create 3 new folders called, 'lang, skinpacks, textures' and a text file renamed to 'skin_packs.json'

### Step 9
Inside skinpack create a new folder and rename it to 1, inside this folder add ALL '.cpmmodel' you want inside that pack.

### Step 10
Inside Textures, create another folder called 'skinpack_icons' and add a image you want to be displayed in-game as the pack icon. for ideal sizes use 1000x1000 or 500x500.

### Step 11
Lang folder is used for translation, so add the lang text doc you want for this example we will use English US, create a text file and rename it to 'en_us.json'

### Step 12
Open 'en_us.json' and add something like this

{
  "skin_pack.ExampleSkinPack.1": "Default Slim",
  "skin_pack.ExampleSkinPack.1.0": "Alex",
  "skin_pack.ExampleSkinPack.1.0.desc": "(Slim)",
  "skin_pack.ExampleSkinPack.1.1": "Ari",
  "skin_pack.ExampleSkinPack.1.1.desc": "(Slim)",
}

'skin_pack.' is the skin_pack folder.
'ExampleSkinPack.' is the pack name from Step 7.
'1' is the skin pack title.
'1.0' is the skins.
1.0.desc' is the description for said skin.

### Step 13
inside 'skin_packs.josn'

{
"ExampleSkinPack:1": {
    "icon": "ExampleSkinPack:textures/skinpack_icons/pack.png",
    "type": "skin",
    "skins": [
      {"model": "ExampleSkinPack:skinpacks/1/slimalex.cpmmodel"},
      {"model": "ExampleSkinPack:skinpacks/1/slimari.cpmmodel"}
  ]
  }
} 
