**Quick Sort** adds a new GUI menu when looting containers and players. Players can choose what type of items they want to put in the container, or even loot all items from the container. Also supports automated looting containers that isn't accepting players items.

## Permissions

- `quicksort.use` -- Allows player to use Quick Sort UI and features
- `quicksort.lootall` -- Allows player use Loot All feature
- `quicksort.autolootall` -- Allows player use Automated Loot All feature

## Commands

This plugin provides both chat and console commands using the same syntax. When using a command in chat, prefix it with a forward slash: `/`.

**Player preferences**
```
/qs  <help | h> - show commands list.
/qs - toggle QuickSort UI.
/qs auto - toggle automated looting.
/qs style "center/lite/right/custom" - change UI style.
/qs container "main/wear/belt" - add/remove container type from the sort (if they are enabled in the configuration).
```

## Configuration

```json
{
  "Use permissions": true,
  "Global settings": {
    "Allows admins to use Quick Sort without permission": true,
    "Default enabled": true,
    "Default UI style (center, lite, right, custom)": "right",
    "Loot all delay in seconds (0 to disable)": 0,
    "Enable/Disable loot all on the sleepers": false,
    "Default enabled container types": {
      "belt": false,
      "main": true,
      "wear": false
    },
    "Excluded containers": [
      "bandit_shopkeeper",
      "bigwheelbettingterminal",
      "dropbox.deployed",
      "npcvendingmachine",
      "npcvendingmachine",
      "npcvendingmachine_attire",
      "npcvendingmachine_building",
      "npcvendingmachine_building",
      "npcvendingmachine_building_hapis",
      "npcvendingmachine_buyres_hapis",
      "npcvendingmachine_components",
      "npcvendingmachine_food_hapis",
      "npcvendingmachine_hapis_hapis",
      "npcvendingmachine_resources",
      "npcvendingmachine_tools",
      "npcvendingmachine_weapons",
      "npcvendingmachine_weapons_hapis",
      "shopkeeper_vm_invis",
      "shopkeeper_vm_invis",
      "vending_mapmarker",
      "vendingmachine.deployed",
      "wall.frame.shopfront",
      "wall.frame.shopfront.metal",
      "wall.frame.shopfront.metal.static"
    ],
    "Auto loot all enabled by default?": true
  },
  "Custom UI Settings": {
    "AnchorMin": "0.637 0",
    "AnchorMax": "0.845 0.146",
    "Color": "0.5 0.5 0.5 0.33",
    "ButtonsColor": "1 0.5 0 0.5",
    "LootAllColor": "0 0.7 0 0.5",
    "TextColor": "#FFFFFF",
    "TextSize": 16,
    "CategoriesTextSize": 14
  },
  "Chat settings": {
    "Chat command": [
      "qs",
      "quicksort"
    ],
    "Chat prefix": "<color=#00FFFF>[Quick Sort]</color>: ",
    "Chat steamID icon": 0
  }
}
```

## Localization

```json
{
  "Deposit": "Deposit",
  "DepositAll": "All",
  "DepositAmmo": "Ammo",
  "DepositAttire": "Attire",
  "DepositConstruction": "Construction",
  "DepositExisting": "Existing",
  "DepositFood": "Food",
  "DepositItems": "Deployables",
  "DepositMedical": "Medical",
  "DepositResources": "Resources",
  "DepositTools": "Tools",
  "DepositTraps": "Traps",
  "DepositWeapons": "Weapons",
  "DepositComponents": "Components",
  "DepositMisc": "Misc",
  "LootAll": "Loot All",
  "NotAllowed": "You do not have permission to use this command",
  "Enabled": "<color=#228B22>Enabled</color>",
  "Disabled": "<color=#B22222>Disabled</color>",
  "SyntaxError": "Syntax error, type '<color=#FFFF00>/{0} <help | h></color>' to view help",
  "QuickSort": "Quick Sort GUI is now {0}",
  "Style": "Quick Sort GUI style is now {0}",
  "AutoLootAll": "Automated looting is now {0}",
  "ContainerType": "Quick Sort for container type {0} is now {1}",
  "Help": "List Commands:\n<color=#FFFF00>/{0}</color> - Enable/Disable GUI.\n<color=#FFFF00>/{0} auto - Enable/Disable automated looting.\n<color=#FFFF00>/{0} style \"center/lite/right/custom\" - change GUI style.\n<color=#FFFF00>/{0} conatiner \"main/wear/belt\" - add/remove container type from the sort."
}
```

## Credits

- **emu**, for the original version of this plugin
- **Wulf**, the original author of the re-written version of this plugin