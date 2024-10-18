# FanLore Features
> "FanLore" is the current working title, and not necessarily the final app name.

## Screens
The major screens within the appp, each screen is accessible from the main menu. Various Tool Windows (see below) add selector and editing capabilities to each specific screens.

### Generic
These screens have no intrinsic knowledge of  any game world or system.

* **Welcome / Setup** - Scans a selected folder for PDF files that match your preferred naming convention. It will build a catalog of the matching PDFs and extract certain metadata including a cover art image from anywhere on the first page, an image of the entire first page, all the text from the document for keyword searching.
* **Explore Content** - Allows the user to browse the PDF content that was discovered by the *Welcome/Setup* screen. Only basic information about the content is displayed, such as page count, and extracted images, along with a 3D rendering of the content as a book. The original PDFs can be launched from this screen in the users preferred PDF reading application (e.g. Acrobat Reader, default web browser etc.). [see below for Hârn specific features]
* **Map Tile Editor** - Allows you to crop any existing images that you have, this includes the images of the first page of a PDF, which is useful for creating rasterized images of PDF maps.
* **Map Editor** - Defines maps that can be used within the *Map Viewer* (see below). Each map has a name, area and any number of layers. Each layer can be comprised of any number of map tiles and has an associated zoom range at which its visible. This allows overview maps which will then fade out as the map is zoomed in to reveal high definition content from other layers. In addition to image tiles there are various other map layer presets such as grid lines and hexes. Maps definitions can be saved to the users preferred folder.
* **Map Viewer** - Render the maps defined by the *Map Editor*. The viewer allows the maps to be zoomed and panned via the mouse. When used in conjunction with *Location Selector* it also supports jumping to known locations and showing addition location details.
* **Settings** - Standard screen for choosing user preferences such as light/dark mode and default locations to store content produced by the app (like generated characters).

### Hârn Specific
These screens are designed around some aspect of the Hârn World system.

* **Home** - Creates a landing page used when opening the app. There's no real functionality available, it just provides some summary statistics about your collection and renders a randomly sequenced montage of publications. Some of the statistics are generic, like number of publications (PDFs), page count, art count etc., but some are Hârn specific for example: kingdom with most modules owned, number of maps publications, kingdom not yet collected etc.
* **Explore Content** - The majority of the details are generic and could apply to any PDF document. However, the screen also tries to place the content to a location on Hârn, and is automatically tagged based on the known list of Columbia Games titles. For example it will derive a publication reference from the PDF file name, from there it knows that numbers in the range 5770-5799 are likely Thardic Republic modules. In addition the 3D render mimics the hardcover books, or the website module images, and includes a Columbia Games logo.

### HârnMaster Specific
These screens are build exclusively to work with the HârnMaster rule system. The include coded versions of the rules contained within the books in order to provide the ability to generate compatible characters and combat simulations.

* **Character Generation** - Allows for the creation and saving of HârnMaster (V3) characters. Characters can be entirely manually generated, for example copied from an existing character sheet; fully randomly generated - click a button to create a character ready to equip; using the Character Point system defined in the rules; or by simulating dice rolls [or any combination of these].
* **Character Sheets** - Allows the users catalog of generated characters to be browsed and edited. Characters are displayed in a fashion similar to the official character sheets, but tool windows provide the ability to edit almost every aspect of the character. It is from here also that the character can be equipped with weapons, armour and sundry equipment. All derived attributes and skill stats are updated as you edit.
* **Combat Simulation** - Provides the ability to simulate combat between multiple teams over a set number of very simplistic arenas (this may be expanded in future to include an editor). Combat is performed in turns and follows as best as possible my interpretation of the HârnMaster combat rules. Many (but certainly not all) optional rules are configurably included, such as weapon damage, tactical advantages, amputations, knockbacks etc.
* **Gameplay** - This settings screen allows the user to select which HârnMaster optional rules they wish to include in character generation, sheets and combat simulations. Not all optional rules are implemented, but those that are may be toggled on/off to suit the users preferences. 

## Tool Windows
These windows appear docked to the right side of the app. They interact with the current screen that is displayed by providing the ability to select, search or edit content.

### Generic
<!--
| | |
|-|-|
| **Map Selector** - Simple tool that allows you to select from any of the existing maps, or to load a previously saved map definition from a folder. | <a href="./Features/Screenshot%20-%20Map%20Selector.png"><img src="./Features/Screenshot%20-%20Map%20Selector.png" width="200"></a> |
| **Map Layers** - When a map is selected and displayed on the *Map Viewer* screen this tool window allow the various layers to be toggle on/off. Toggling a layer off makes it invisible. Note that individual layers within the map's definition can configure their own default for this toggle (some layers can be off by default). | <a href="./Features/Screenshot%20-%20Map%20Layer%20Selector.png"><img src="./Features/Screenshot%20-%20Map%20Layer%20Selector.png" width="200"/></a> |
| **Document Search** - Keyword search across the text content of all PDF documents in the catalog (created during *Welcome/Setup*). | <a href="./Features/Screenshot%20-%20Document%20Search.png"><img src="./Features/Screenshot%20-%20Document%20Search.png" width="200"></a> |
-->

* **Map Selector** <a href="./Features/Screenshot%20-%20Map%20Selector.png">
<img src="./Features/Screenshot%20-%20Map%20Selector.png" width="80" style="float: right;">
</a> - Simple tool that allows you to select from any of the existing maps, or to load a previously saved map definition from a folder.

* **Map Layers** <a href="./Features/Screenshot%20-%20Map%20Layer%20Selector.png"><img src="./Features/Screenshot%20-%20Map%20Layer%20Selector.png" width="80" style="float: right;"/></a> - When a map is selected and displayed on the *Map Viewer* screen this tool window allow the various layers to be toggle on/off. Toggling a layer off makes it invisible. Note that individual layers within the map's definition can configure their own default for this toggle (some layers can be off by default).

* **Document Search** <a href="./Features/Screenshot%20-%20Document%20Search.png"><img src="./Features/Screenshot%20-%20Document%20Search.png" width="80" style="float: right;"></a> - Keyword search across the text content of all PDF documents in the catalog (created during *Welcome/Setup*).

## Hârn Specific
These Tool Windows are specific to Hârn because they have intrinsic knowledge about various official publications. Such as categorizing content, knowing the map co-ordinates of kindoms, settlements, towns and trade routes. In some instances even having a detiled knowledge base on individual settlements.

* **Module Selector** <a href="./Features/Screenshot%20-%20Module%20Selector.png"><img src="./Features/Screenshot%20-%20Module%20Selector.png" width="80" style="float: right;"></a> - Selects a PDF publication based on its name and number. The publication's are those that are part of the users own catalog (discovered during *Welcome/Setup*) but will be tagged based on conventions used by Columbia Games, e.g. 5740-49 associated with "Kingdom of Rethem" tag.

* **Location Selector** <a href="./Features/Screenshot%20-%20Location%20Selector.png"><img src="./Features/Screenshot%20-%20Location%20Selector.png" width="80" style="float: right;"></a> - Selects a settlement based on its name and tags. Settlments co-ordinates and details are included in the dataset used by the app and this is specific/copyrighted to Hârn. For example tags include the Kingdom/Area, Location type, etc. 

*  **Location Editor**  <a href="./Features/Screenshot%20-%20Location%20Editor.png"><img src="./Features/Screenshot%20-%20Location%20Editor.png" width="80" style="float: right;"></a> - Shows extended metadata that may exist for specific settlements. This data has been copied directly from Columbia Games' Kingdom books and stored in program assets.

## HârnMaster Specific
These Tool Windows are specific to the HârnMaster rule system. They work in conjunction with the Character Generation and Character Sheet screens. They require  knowledge of the Character, Skills, Magic and Religion rules together with tables for armour, weapons, skills, sunsigns, occupations, birthplaces, etc.

* **Character Armour Editor** - Add armour to the selected character, or edit existing armour attributes. In addition to selecting armour material and garment it allows for customizing armour quality and weight.

* **Character Weapon Editor** - Add new weapons to the selected character, or editing existing weapon attributes. In addition to selecting weapon class and type it allows for customizing weapon quality and weight, and even supplying a unique name.

* **Character Skill Editor** - Add new skills to the selected character, or edit existing skill mastery levels. It will also show a detailed breakdown of skill base calculations including stats and sunsign modifiers.

* **Character Points** - Keeps track of *Character Point* spending when using the optional rules provided by HârnMaster for generating characters in this manner. Both core and extended character point groupings are supported.
  
* **Character Selector** - Lets you browse the characters in your default character folder (as configued in *Settings* screen). You can also load files from any other folder.

