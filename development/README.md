This website documents the "types" of Wayward — basically, the structure of the game's code.

## Finding an export
Sometimes, while modding, you'll see examples which reference something you don't have, such as `ItemType`,
and VSCode will put a red underline under it because you haven't imported it yet. In cases where VSCode is unable to automatically
import it for you, you can find the path in this documentation.

Clicking on the magnifying glass icon at the top allows you to search the documentation for the export you're looking for.
In the case of `ItemType`, one of the suggestions is `game/item/IItem.ItemType`. Clicking on it goes to the definition.

Your import will be `import { NAME } from "PATH";`, where NAME is the export you were looking for (ie `ItemType`),
and PATH is the text of the *second* link in the breadcrumbs (ie at the top it might say, for example, __Wayward Types Viewer__ / __game/item/IItem__ / __ItemType__ /).
For example `import { ItemType } from "game/item/IItem";`.

Some imports will be the "default" export from a module. In that case the import will be, for example, `import Register from "mod/ModRegistry";`
Notice how the import is the name without the `{}` curly braces.


## Other tips to using this site

The [Module Index](./modules.html) contains a list of every single file in the game, and therefore all possible paths for you to import from.

The **Common Modules** section of the sidebar lists some commonly-referenced things for Wayward modding. Take a look!

You can visit https://waywardgame.github.io/development/ to see a copy of the types specific for the "development" branch in the Steam betas.


# Need help?

## Wayward Modding Guide
**https://github.com/WaywardGame/types/wiki — If you're new, start here!**

## Documentation
* `+mod create` & `+mod update` — https://github.com/WaywardGame/types/wiki/mod-create-&-update
* `mod.json` — https://github.com/WaywardGame/types/wiki/mod.json
* Extracting assets — https://github.com/WaywardGame/types/wiki/Extracting-Wayward-Assets

## Mod Content
* Script mods — https://github.com/WaywardGame/types/wiki/Script-Mods
* Language mods & adding language to script mods — https://github.com/WaywardGame/types/wiki/Languages-&-Extensions
* Customizations (hair styles, hair colours, skin tones) — https://github.com/WaywardGame/types/wiki/Customizations
* Image Overrides (replacing sprites & textures) — https://github.com/WaywardGame/types/wiki/Image-Overrides
* Stylesheets (changing the appearance of the UI) — https://github.com/WaywardGame/types/wiki/Stylesheets


## Other useful quick-links:

* Modding Examples: https://github.com/WaywardGame

* Steam Workshop: http://steamcommunity.com/app/379210/workshop/

* Wayward Types Viewer: https://waywardgame.github.io/ — A pretty, searchable website documenting all the "types" of Wayward. If you need to figure out how to do something, or want to see your options, try searching for it on this site! 
  * Expert users can feel free to search the raw files here: https://github.com/WaywardGame/types/tree/master/definitions
  * After you have a development environment set up, you can also look in node_modules/@wayward/types/definitions in your mod's directory.