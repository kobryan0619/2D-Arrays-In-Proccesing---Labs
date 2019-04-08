## LAB #3: Multiple Images
Once you understand how to manipulate the pixels in one image, you can copy pixels from one picture to another. 

1. The code below compares two colors and returns true if they are "similar". Take a look at the code and make sure you understand how it is working. How could you adjust the threshold if to make the comparison more or less sensitive? Once you understand how the code works, use it to replace the green screen behind the cat with the explosion picture. 

```
boolean closeColor(color c1, color c2){
    double distance = (red(c1) - red(c2))*(red(c1) - red(c2)) + (green(c1) - green(c2))*(green(c1) - green(c2)) + (blue(c1) - blue(c2))*(blue(c1) - blue(c2));
    if(distance < 250){
        return true;
    }else{
        return false;
    }
}
```

![A cat on a green screen](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/cat1.jpg)
![An explosion](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/explode.jpg)

![The explosion as the background of the cat picture](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/greendone.png)

2. Put a bowtie on Grumpy Cat

![Grumpy Cat](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/grumpy.jpg)
![Grumpy Cat with a bowtie](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/grumpy2.png)

3. Create a collage using at least five images. To do this, first write a method that will allow you to place one image on another at a specified location. Once you have the collage code working (1) modify pictures (e.g. add a colored filter) before you put them on the collage (2) try to add one image veritacally rather than horizontally.

![A collage of animal pictures](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/collage.jpg)
