.. todo::

   This page is still work in progress.

Create a map
============

This is how you create a custom map for IW4x.

Requirements
------------

You have to fulfill the following requirements to be able to create a custom
map for IW4x:

-  A clean installation of `Call of Duty: Modern Warfare
   2 <http://store.steampowered.com/app/10180>`__
-  A clean installation of `Call of Duty 4: Modern Warfare
   <http://store.steampowered.com/app/7940>`__
-  The latest `mod tools
   <https://www.google.com/search?q=Call+of+Duty+4:+Modern+Warfare:+Mod-Tools>`__
   for *Call of Duty 4*
-  The latest **IW4x client** installed in your *Modern Warfare 2* directory
-  The latest **IW3 exporter** installed in your *Call of Duty 4* directory
-  The latest **IW4x Mod-Builder** and both your *Call of Duty 4* and *Modern Warfare
   2* paths configured in the settings

Create a map
------------

| Creating a custom map requires to create a map for *Call of Duty 4* first.
| For that you can follow various existing `tutorials <http://wiki.modsrepository.com/index.php?title=Call_of_Duty_4:_mapping_mp>`__.
| You can then follow the steps to convert your map for IW4x.
|

Convert a map
-------------

Notes
~~~~~
-  Automatic conversion for now only works for multiplayer maps
-  Your map might have a lot of bugs, map conversion is in an early alpha stage
-  Once we update the tools, you might have to reconvert your map

Conversion
~~~~~~~~~~
* Open the *Build Map* tab in the **IW4x Mod-Builder**
* You will see a list of maps if you correctly configured all paths:

   * **Stock Maps** are the maps located in your ``<Call of Duty 4>/zone/<language>/`` directory
   * **User Maps** are the maps located in your ``<Call of Duty 4>/usermaps/`` directory
   * **Other Maps** are the maps you already converted, they will be in your
     ``<Modern Warfare 2>/mods/`` directory

* Select the map you want to convert and click *Export COD4 Map*, this will
  export all required files into your ``<Modern Warfare 2>/mods/`` directory
* After the export, you can optionally edit the map's CSV source [1]_ or edit the
  arena to change the name or teams of your map.
* Click on *Build MW2 Map* to create the map, it will be located in ``<Modern Warfare 2>/usermaps/``
* At this point, you are able to test your map by clicking *Run MW2 Map*

Deployment
~~~~~~~~~~
| Once you followed all the steps for converting your map, you have to generate the IWD
| by clicking *Generate IWD* for the map you selected in the **IW4x Mod-Builder**. This will compress the images for your map.
| All required files should be located in ``<Modern Warfare 2>/usermaps/<your map>/``.
| Those are all files you need, you can then run the map on your server or client using ``map <your map>``.
| Players connecting to your server will automatically download all required ressources to play the map.
| 

.. [1]
   Sometimes, you will get missing techset errors.
   This means you will need other dependency maps in your CSV.
   For now, as it is still hard to find the correct dependency, you can contact the IW4x staff on discord.
