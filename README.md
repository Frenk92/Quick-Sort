**Quick Sort** adds a new GUI menu when looting containers and players. Players can choose what type of items they want to put in the container, or even loot all items from the container.

## Permissions

- `quicksort.use` -- Allows player to use Quick Sort UI and features
- `quicksort.lootall` -- Allows player use Loot All feature

## Commands

**Player preferences**
```
/qs help - show commands list.
/qs enabled "true/false:OPTIONAL" - enable/disable QuickSort UI.
/qs style "center/lite/right/custom" - change UI style.
/qs container "main/wear/belt" "true/false:OPTIONAL" - add/remove container type from the sort (if they are enabled in the configuration).
```

## Configuration

```json
{
  "Default UI style (center, lite, right, custom)": "right",
  "Loot all delay in seconds (0 to disable)": 0,
  "Enable/Disable loot all on the sleepers": false,
  "Enable/Disable container types": {
    "Main": true,
    "Wear": false,
    "Belt": false
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
  "LootAll": "Loot All",
  "DepositComponents": "Components",
  "DepositMisc": "Misc",
  "InvalidArg": "\"{0}\" is an invalid argument.",
  "Edited": "\"{0}\" edited to: {1}",
  "Help": "List Commands:\n/qs enabled \"true/false\" - enable/disable gui.\n/qs style \"center/lite/right/custom\" - change gui style.\n/qs conatiner \"main/wear/belt\" \"true/false\" - add/remove container type from the sort."
}
```

## Credits

- **emu**, for the original version of this plugin
- **Wulf**, the original author of the re-written version of this plugin