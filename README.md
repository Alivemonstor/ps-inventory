# PS-Inventory Alivemonstor's Edit

lj-Inventory has been fully redesigned by [OK1ez](https://github.com/OK1ez), under the name ps-inventory. This has now been updated by me to support a different look and added support for as many monitor sizes as i could find.

Future updates will be coming and we will of course support all normal monitor sizes.

# Previews

### Simple item guidelines (found in main directory ps-inventory)

![ps-inventory Guideline](https://user-images.githubusercontent.com/91661118/146315681-c67f542d-e2bc-43ca-9957-7f1971b84268.png)

### Full Inventory

![image](https://cdn.discordapp.com/attachments/845269951312166942/1190985802189115455/image.png?ex=65a3caf6&is=659155f6&hm=be89825469500cf2b6270da4926fa90333a57ce18b12c70bad7c2bd62cd4a8fc&)


### Hotbar Slots

![image](https://cdn.discordapp.com/attachments/845269951312166942/1190986030866780240/image.png?ex=65a3cb2d&is=6591562d&hm=92ea1f6a054cb1df000d7f42c54e075479dc45a5c57fe4708cc89943d66c9119&)

### Inventory Glovebox

![image](https://cdn.discordapp.com/attachments/845269951312166942/1190986122583613520/image.png?ex=65a3cb43&is=65915643&hm=4b172aa4e5eed64ad897c49b758a7b644f32c419d75890bffff70a9ddc8bc2e1&)

### Inventory Trunk

![image](https://cdn.discordapp.com/attachments/845269951312166942/1190986298643709972/image.png?ex=65a3cb6d&is=6591566d&hm=1a150f5953c59afc53549e1f310b1b1d821e77a4bec7db24149f95513d27e1d7&)

# Key Features

* ALL IMAGES FOLLOW THE SAME DIMENSIONS
* Easy Photoshop guideline template for creating custom images within ps-inventory
* Custom brand logo above option buttons
* Options menu
* Help box 
* Custom inventory images (more always being added in each new update)
* Default weight icon easily changeable with Font Awesome icons
* Hotkey numbers visible in inventory and hotbar slots
* Weight progress bar
* Tooltip has a determined height (so it won't ever go higher than visible or cut off)
* Text overflow ellipsis used (so your product titles with never overlap the containers and instead do "...")
* Blurred inventory background
* Elements of NoPixel 3.5 design ideas interwoven

# How to install ps-inventory (Latest QBCore Update)

* Download `ps-inventory` from our GitHub
* Make sure you have the latest update of [qb-core](https://github.com/qbcore-framework/qb-core)
* Make sure you have the latest update of [qb-smallresources](https://github.com/qbcore-framework/qb-smallresources)
* Make sure you have the latest update of [qb-weapons](https://github.com/qbcore-framework/qb-weapons)
* Drag `ps-inventory` into your resources folder or any subfolder
* Make sure that the folder is named `ps-inventory` and **not** `ps-inventory-main`
* Replace all occurrences of `qb-inventory` with `ps-inventory`.<br>The example below uses Visual Studio Code to replace all instances.

![image](https://github.com/Z3rio/ps-inventory/assets/54480523/00fa21a5-4be2-443f-aff2-4b3202b662dc)

## Set up the decay system

If you want the decay system to work, then please read the information below, otherwise it won't work.

You need to add a decay value for all items in your `qb-core/shared/items.lua` file, the variable stands for the number of days it takes to decay.

### Examples:

#### Example of what you have to add

```lua
-- decay = The number of days it takes for an item to decay
-- delete = If set to true, the item will be removed once it decays
["decay"] = 28.0, ["delete"] = true
```

#### Example with the full item in QB-Core's shared file

```lua
['sandwich'] = {['name'] = 'sandwich', ['label'] = 'Sandwich', ['weight'] = 200, ['type'] = 'item', ['image'] = 'sandwich.png', ['unique'] = false, ['useable'] = true, ['shouldClose'] = true,	['combinable'] = nil, ['description'] = 'Nice bread for your stomach', ["decay"] = 3.0, ["delete"] = true},
```

In this example, the sandwich item would take 3 days to decay and once it does, it would be removed.

# Dependencies

* [qbcore framework](https://github.com/qbcore-framework)
* [qb-target](https://github.com/BerkieBb/qb-target)
* [qb-core](https://github.com/qbcore-framework/qb-core)
* [qb-logs](https://github.com/qbcore-framework/qb-logs)
* [qb-traphouse](https://github.com/qbcore-framework/qb-traphouse)
* [qb-radio](https://github.com/qbcore-framework/qb-radio)
* [qb-drugs](https://github.com/qbcore-framework/qb-drugs)
* [qb-shops](https://github.com/qbcore-framework/qb-shops)

## Performance

Runs at ~ 0.00 to 0.01 ms if you have more optimization suggestions feel free to reach out

# Credits
* Alivemonstor for Updated [Redesign](https://github.com/Alivemonstor)
* [OK1ez](https://github.com/OK1ez) for full Initial redesign. 
* ihyajb (Aj) for [original version](https://github.com/ihyajb/aj-inventory)
* Jay for [decay](https://github.com/tnj-development/inventory)
* i-kulgu for [updated decay](https://github.com/i-kulgu/qb-inventory-decay)
* [OnlyCats](https://github.com/onlycats) who helped reorganize and also created some custom images.

# Issues and Suggestions

Please use the GitHub issues system to report issues or make suggestions, when making suggestions, please keep [Suggestion] in the title to make it clear that it is a suggestion.

## Connect with us

Join our [**Discord**](https://discord.gg/vH4eFZkkp) for updates, support, and other scripts
