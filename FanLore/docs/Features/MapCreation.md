# Creating a Map

The following guide walks you through how to create and save a new map using imagery extracted from PDF content.

## A note on extracting images from PDF
In order for Fanlore to extract high resolution images from the PDF files that can be used as map tiles you will need to install Ghostscript. See information about installing Ghostscript [here](../ReadMe.md).

If you don't want to install Ghostscript then you can still create maps tiles, you will just need to generate your own jpg/png files from the PDF content.

## Create a Hârn Map

To create your own zoomable map of Hârn:

1. Download the free map of Hârn from Columbia Games website. The is one of the most iconic maps in fantasy gaming, and often the lure that attracts folks to the world of Hârn in the first place.
2. Once downloaded you should have a file with a name simialr to `5001A-HarnWorld-Map_Bilbo.pdf`. Open the PDF and view the map to make sure it downloaded correctly.
3. Launch FanLore.
4. Copy the downloaded file into your "Official Content" folder. This is the folder that FanLore expects to find PDFs. 
   1. If FanLore is running while you copy the PDF into your "Official Content" folder then it will automatically scan the file and inform you of new content.
   2. If FanLore is not running then the next time you launch it will still see the new PDF file, but it won't extract and details. You can use the Welcome screen's "Perform Search" button to scan all content and pick up the new imagery.
5. Open the *Map Tile Editor* in FanLore.
6. From the right hand tool panel you should be able to select the map you downloaded. If the naming convention matches that from step 2 then it will appear as *HarnWorld Map* with a publication reference of *5001A*. It may take a few seconds to load the image of the PDF.
7. When creating tiles you can extract an image as a single file, or you can split the images into many tiles. Creating many smaller tiles helps the application's performance since it can optimize which tiles to draw and not have to deal with the entire map as your zoom. For the Hârn map its ideal to set the mode from *Single* to *Multiple*. The app should automatically detect that this is a 14 x 10 map, just based on the publication reference. In this case it will be set to create 140 map tiles.
8. Before you can generate the tiles you need to tell the app what area of the PDF you wish to convert to tiles. There is a rectangle overlaid on the PDF image, you can drag the corners of the overlay to match the interior corners of the map. Note that as you drag the corners they zoom to better help you align to the map edges. In addition, when using *Multiple* tile mode the overlay will show the boundaries of each tile. Position the overlay so that it aligns to the corners of the map, and the tile boundaries also align to the map squares.
9. Once everything is aligned correctly click the *Generate 140 Map Tiles* button. It will take a few seconds and then you should see a message telling you how many tiles were created and where they were saved.
10. Now switch to the *Map Editor* screen.
11. Click the dropdown arrow or on the instruction text to expand the panel to show the buttons.
12. Enter a map name, e.g. "My Hârn Map"
13. Enter the dimensions covered by the map. Don't worry too much about this yet, but the best default is "50.000°N, 0E 1400km x 1000km    ". This may not be entirely accurate, but gives a good starting point.
14. Enter an aspect ratio of "1.03923048", believe it or not those map squares aren't...  square.
15. You can optionall pick a background color, this is useful if you're dealing with PNG files that have transparency.
16. Pick on of the projections, don't worry too much about this you can change it later. It will determine how longitude and latitude are calculated from the map X/Y co-ordinates.
17. Click the *New Map* button. The Edit Map Layers section will now appear below the map details. By default there are two map layers (Highlights and Debug). You should keep the Highlights layer, it determine which layer is used to draw towns, boudnaries, text etc. on your map. The layers are sequenced in the order they are drawn. The Highlights layer should be one of the last layers drawn, otherwise it will be obscured by later layers.
18. Add a new layer by clicking the drop down next to *Add Image Layer*. Select *Add Tiled Image Layer*.
19. Move the layer to the top using the *up* arrow button.
20. Give the layer a description e.g. "5001A Map Tiles". Leave the layer extent as the default (it will fill map). Change the *Tile file name prefix* to *5001A* (assuming that was the name used to prefix the tiles you generated, if you created your own tiles then modify to match).
21. Use the...   
22. Click the *Save Map...* button, and accept the default save location which should be the *FanLore\Maps* folder.  