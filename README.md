# Haven&Hearth global map hashed tiles 

## Description 
all map tiles are downloaded from [https://odditown.com/haven/map/](https://odditown.com/haven/map/); 

every png-tile is converted to a bitmap using [YAPD](https://github.com/kyriosli/YAPD), because canvas gives different results for different browsers; 

Locality Sensitive Hash [TLSH](https://github.com/trendmicro/tlsh) is used for fuzzy matching tiles; 

when user drag-n-drops a tile, it is converted to a bitmap and matched against generated hash database to show coordinates of this tile on a global map.

## How to use 
you spawned in the wild and wanna know your coordinates on a global map; 

turn on "save to disk" tiles in your client and drag-n-drop a tile (or few) from current game-session to the "Drop files here" zone; 

press Search button to download ~9Mb hashes (2.8Mb gzipped) and match your tile hash against them; 

results with difference < 100 are saved and are filtered by slider value (10 by default). 
