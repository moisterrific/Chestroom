# Chestroom
Chestroom containing all ingame items

this plugin generates a chestroom containing all the items that are currently in the game.
By default the shape of the room will always be (if possible) a square
Torches, bakcground, tiles, chests and platforms are customizeable, or otherwise at random.
If using infinite chests plugin, all the chests will automagicly refill.
If CustomRoom is set to false, Everything will be at random.
Will not require any updates when more items are brought into the game ;D
Commands
/chestroom (or /cr) <tl/tr/bl/br/tc/bc> | Place a chestroom based on your position. (see below for more info)
/crreload | Reload the chestroom config file.
More info about chestroom command
t = top
l = left
r = right
b = bottom
c = center

For example if you use /chestroom bc, you will stand at the bottom center of the chestroom when it spawns.

Config File
Code:
{
    "ChestsPerRow": 9, //# of chests per row, cannot go below 1 or higher than # of chests needed (currently 90).
    "CustomRoom": false, //If true it will use the options below.
    "TileId": 38, //The tile type used for the chestroom.
    "ChestId": 1, //Chest type.
    "BgWall": 4, //Background wall id.
    "pFrameY": 18, //All platforms have the same item id, so you modify them by changing the Frame Y.
    "tFrameY": 22 //All torches have the same item id, so you modify them by changing the Frame Y.
}

chestroom.create - for usage of /chestroom (or /cr)
chestroom.reload - for usage of /crreload 
