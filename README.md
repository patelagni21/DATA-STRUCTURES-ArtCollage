# DATA-STRUCTURES-ArtCollage

ArtCollage (110 points). The ArtCollage class create a collage of image tiles and provides methods to transform the tiles individually. See ArtCollage.java for the description of each method.

One-argument Constructor
ArtCollage art = new ArtCollage(args[0]);
art.showCollagePicture();

The original image (args[0]) has 1536 rows x 1819 columns. The collage image that results from the one-argument constructor (on the left) has 400 rows by 400 columns.

Three-argument Constructor
ArtCollage art = new ArtCollage(args[0], 200, 3);
art.showCollagePicture();

The original image (args[0]) has 1536 rows x 1819 columns. The collage image that results from the three-argument constructor (on the left) has 600 rows by 600 columns.

MakeCollage method
// Creates a collage of 3x3 tiles. 
// Each tile dimension is 200x200 pixels.
ArtCollage art = new ArtCollage(args[0], 200, 3);
art.makeCollage();
art.showCollagePicture();
// Creates a default collage of 4x4 tiles. 
// Each default tile dimension is 100x100 pixels.
ArtCollage art = new ArtCollage(args[0]);
art.makeCollage();
art.showCollagePicture();


Change Tile Methods
// Creates a collage of 3x3 tiles. 
// Each tile dimension is 200x200 pixels
ArtCollage art = 
  new ArtCollage(args[0], 200, 3);

art.makeCollage();

// Colorize tile at col 2, row 2 
// to only show the red component
art.colorizeTile("red",2,2);
art.showCollagePicture();
// Creates a collage of 3x3 tiles. 
// Each tile dimension is 200x200 pixels
ArtCollage art = 
    new ArtCollage(args[0], 200, 3);

art.makeCollage();

// Colorize tile at col 2, row 1 
// to only show the blue component
art.colorizeTile("blue",2,1);
art.showCollagePicture();
// Creates a collage of 3x3 tiles. 
// Each tile dimension is 200x200 pixels
ArtCollage art = 
     new ArtCollage(args[0], 200, 3);

art.makeCollage();

// Colorize tile at col 0, row 0 
// to only show the green component
art.colorizeTile("green",0,0);
art.showCollagePicture();



// Creates a collage of 3x3 tiles. Each tile dimension is 200x200 pixels
ArtCollage art = 
    new ArtCollage(args[0], 200, 3);

art.makeCollage();

// Converts the tile at col 1, row 0 
// from color to greyscale
art.grayscaleTile(1, 0);
art.showCollagePicture();
// Creates a collage of 3x3 tiles. 
// Each tile dimension is 200x200 pixels
ArtCollage art = 
  new ArtCollage(args[0], 200, 3);

art.makeCollage();

// Replace tile at col 1, row 1 with 
// args[1] image
art.replaceTile(args[1],1,1);
art.showCollagePicture();


Note: Make sure to test colorizeTile() and greyscaleTile() using a collage where each tile has a different image.

ArtCollage art = new ArtCollage(args[0], 200, 2);
art.makeCollage();

// Replace 3 tiles 
art.replaceTile(args[1],0,1);
art.replaceTile(args[2],1,0);
art.replaceTile(args[3],1,1);
art.colorizeTile("green",0,0);
art.showCollagePicture();
