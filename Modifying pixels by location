## LAB #2: Modifying pixles by location
In the previous lab we saw how we could uniformly modify all the pixels in an image. However, often, we want to modify a pixel depending on it's location in the image. In this case, we can use the x and y coordinates of a pixel to locate it in the source image. 

Run this code and look at how it modifies your image. Make sure you understand how the loops are working

```
PImage img;

void setup() {
  size(200,200);
  img = loadImage("dino.jpg"); // replace "dino.jpg" with an image of your choice
}

void draw() {
  image(img,0,0);
  loadPixels();
  // Loop through every pixel column
  for (int x = 0; x < width; x++) {
    // Loop through every pixel row
    for (int y = 0; y < height; y++) {
      // Use the formula to find the 1-dimesional location
      int loc = x + y * width;
      float r = red(img.pixels[loc]);
      float g = green(img.pixels[loc]);
      float b = blue(img.pixels[loc]);
      if (x % 2 == 0) { // If we are an even column
        pixels[loc] = color(255, g, b);
      } else {          // If we are an odd column
        pixels[loc] = color(r, g, 255);
      }
    }
  }
  updatePixels();
}
```
Now try the following modifications to portions of an image
1. Download the image of a beach on the left. Modify only the top portion so that the sky looks like a sunset (see the image on the right)

![A picture of a beach with a palm tree](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/beach.jpg)
![The same beach with a pink sky for sunset](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/sunset.png)

2. Duplicate the top half of the image on the bottom

![A picture of a beach with a palm tree](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/stack.png)

3. Mirror the top half of the image

![A mirrored picture of a beach with a palm tree](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/reflect.png)

4. Help this dog caught in the act of stealing the Thanksgiving turkey maintain his anonymity by covering his face with a square.

![A dog stealing a turkey](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/dog.jpg)
![A dog stealing a turkey with a box over his face](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/baddog.png)

