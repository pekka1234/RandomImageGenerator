# ImageGenerator

## What is it?

Image Generator is a command line tool written in C++ to create bitmap images randomly or by input. 

Note: When you view images generated with this program, turn image smoothening off when zooming so you can see the pixels.

Here are some example images that are generated using this program:

Note: some images are screenshots of the actual images because they are so small.

![Screenshot from 2022-12-05 18-23-51](https://user-images.githubusercontent.com/62663286/208254655-1d2ab30b-c047-4c88-b0c2-49a120879f44.png)
![Screenshot from 2022-12-17 19-45-43](https://user-images.githubusercontent.com/62663286/208254662-cc479d23-a324-40c5-b949-a4e9916120ad.png)
![cc](https://user-images.githubusercontent.com/62663286/208254675-4196c62d-4c54-4edb-bb4a-06fd5b8967ab.png)
![Screenshot from 2022-12-17 19-49-38](https://user-images.githubusercontent.com/62663286/208254792-b40f0fe7-adfd-44e4-8b33-4dc6d49f8106.png)

## How to use it?

Note: When black & white images are explained, there will be given some extra general info too, because color image explanations just include how they are diferent from the black & white images, so read black & white explanations first.

### Creating black & white images by a manually typed order

Here is an image of the terminal after an black & white image is created:

![Screenshot from 2022-12-17 19-55-19](https://user-images.githubusercontent.com/62663286/208255073-8e22925d-1e5e-457e-a299-f32967cbbd66.png)

Here is the above image's creation process in steps:

Note: When values are put in the terminal, no spaces are allowed

1. Selecting if image will be black & white (0) or color image (1). In image creation above, black & white (0) was selected.

2. Inserting image' width and height in pixels. In image creation above, 500 was selected to be the width and height.

3. Deciding if image is generated by manually typed order (what orders mean, is explained later on), or randomly (random option includes randomizing color for eachpixel seperately and generating random order by given order length). In image creation above, order 1010100000000000111111111010101 was used.

4. Entering file's name

Note: Steps above are for black and white images generated by manually typed order and for diferent images, the creation steps are diferent, and for those images that are not explained above will be explained later.

#### How black & white image's order work?

Note: Orders are most important and fun thing is this program because the images can look quite interesting.

In this program (when black & white images are used), orders mean sequences of blacks and whites, for example: black,white,white is an order and if that order is put to a 20x20 image, the image would look like this:

![Screenshot from 2022-12-18 10-49-04](https://user-images.githubusercontent.com/62663286/208289288-fb5b5f0a-8c74-4328-b713-f969d3a7781a.png)

In above image you can see that the pixels (starting from up left) are black,white,white,black,white,white... and so on just like the order was (black,white,white) so the orders are just sequences of blacks and white that will fill the image. Orders are inserted to the program in a way that black = 1 and white = 0 so the above image was created using order 100.

Here is the terminal after the above image was created:

Note: pictures from the terminal in this readme are from the first version of this program so the word choises of the questions might have sligtly changed.

![Screenshot from 2022-12-18 10-57-32](https://user-images.githubusercontent.com/62663286/208289594-1bc3373b-a847-47cf-bd86-7a587e29b78e.png)

In the first terminal picture example (where the image creation steps were also explained), the image was 500x500 pixels and had the order 1010100000000000111111111010101. 

Here is the result:

![exmaple_image](https://user-images.githubusercontent.com/62663286/208290124-8b117e7a-984c-4b90-98dc-8ccbfdd49031.png)

The image is quite large (500x500 pixels) so you can't see the pixel structure, but if you zoom in you can see it better:

![Screenshot from 2022-12-18 11-13-57](https://user-images.githubusercontent.com/62663286/208290214-a980ac3e-bb1c-4e0f-a37b-a47589c2f5c0.png)

The pixel structure is in most cases quite interesting and is the fun thing about this program adn if we zoom to the top left of this image, we can see
that the pixel order is being followed:

![Screenshot from 2022-12-18 11-16-29](https://user-images.githubusercontent.com/62663286/208290349-532ed5a3-18a6-4650-88f0-88112853d5b2.png)

Note: The thing that causes those fun pixel structures in the images is the fact that the order's lenght doesn't go evenly to the images width, whcih means that the order will begin from diferent part of the order when looking ti the left side of the image, as seen in the above image.

### Creating color images by a manually typed order

Here is an image of the terminal after a color image is created:

![Screenshot from 2022-12-18 11-29-00](https://user-images.githubusercontent.com/62663286/208290897-5565749e-7c8a-457b-9e3e-e67219af468e.png)

Here is the above image's creation process in steps:

1. Selecting if image will be black & white (0) or color image (1). In image creation above, color (1) was selected.

2. Inserting image' width and height in pixels. In image creation above, 30 was selected to be the width and height.

3. Deciding if image is generated by manually typed order (how color orders work is explained later on), or randomly (random option includes randomizing color for eachpixel seperately and generating random order by given order length). In image creation above, order 000255000,000255000,100100100,255000000 was used.

4. Entering file's name

#### How color image's order works?

Meaning of the word order in this program is explained in the black & white order section, so here will be explained how color image's orders are diferent from the black & white image's order.

First of all, color image's order is a sequence of colors in rgb values, that are seperated by commas, for example the above terminal picture's color order was 000255000,000255000,100100100,255000000 and if those rgb values are translated to english, the colors are: green,green,grey,red.

Here is the result image:

![Screenshot from 2022-12-18 11-45-17](https://user-images.githubusercontent.com/62663286/208291556-2755822a-bc88-4bcc-9afa-904ea421ce8c.png)

Note: the one color's rgb values have always three digits in this program, so for example: 255 = 255, 1 = 001, 35 = 035, 20 = 020... and so on.

### How to create image randomly (both black & white and color work the same way)?

Here is a picture of the terminal after an image is created randomly (using randomization for each pixel seperately):

![Screenshot from 2022-12-18 11-54-55](https://user-images.githubusercontent.com/62663286/208291862-410f8e58-10aa-43f3-b942-b1cdf9616fba.png)

Here is the above image's creation process in steps:

1. Selecting if image will be black & white (0) or color image (1). In image creation above, black & white (0) was selected.

2. Inserting image' width and height in pixels. In image creation above, 50 was selected to be the width and height.

3. Deciding if image is created by manual typed order or randomly. In image creation above randomly (1) was selected.

4. Deciding if randomization for each pixel seperately (0) or random order (1) is used. In image creation above, random for each pixel (0) was selected.

#### How random for each pixel seperately works

Note: Random for each pixel images look all very similiar and the random order is much more fun.

It black & white it basically randomly decides for every pixel that will it be black and white.

In color images it decided random color for each pixel.

Here is the generated image from the above terminal picture:

![Screenshot from 2022-12-18 12-04-59](https://user-images.githubusercontent.com/62663286/208292267-b5073023-ea77-4421-880e-72d8a32268ac.png)

Note: The above image is a screenshot of the actual image (and most of the images you have seen in this readme are also screenshots) because the actual images are so small and because of it beeing a screenshot, you can see a grey pixel in down right corner because it is a bug of my image viewer.

Note: There is a color image of each pixel randomized seperately in the start of this readme.

#### How random order works:

Here is a picture of a terminal after image is created with a random order:

![Screenshot from 2022-12-18 11-54-55](https://user-images.githubusercontent.com/62663286/208292543-1f7e2671-1670-46aa-95bf-15c0e2e5caab.png)

Here is the above image's creation process in steps:

1. Selecting if image will be black & white (0) or color image (1). In image creation above, black & white (0) was selected.

2. Inserting image' width and height in pixels. In image creation above, 100 was selected to be the width and height.

3. Deciding if image is created by manual typed order or randomly. In image creation above randomly (1) was selected.

4. Deciding if randomization for each pixel (0) seperately is used or random order (1). In image creation above, random order (1) was selected.

5. Entering order's lenght. In image creation above, 15 was used

6. Entering file's name

#### How random order works?

For black & white, after the length is given, the program creates a random order that is the given length's amount of pixels long.

For color images the process is same, but instead of zeroes and ones, it randomizes color like 100000213.

After the order is generated, the program says the used order, for example in the terminal picture above: "Used order: 111011011101001".

Here is the generated image from above terminal picture (you can see that the used order is used in that image):

![Screenshot from 2022-12-18 12-22-52](https://user-images.githubusercontent.com/62663286/208293082-1aec15e7-59d0-489a-b7d9-b1356da0cde2.png)

Note: This readme has no example of color image generated by a random order but you can generate that yourself.

## Other information

### When image width is divisible by order length

If that happens, it means that the pixel order will start from the same spot over and over again, resulting bar code style lines.

Here is an example:

![Screenshot from 2022-12-18 12-31-54](https://user-images.githubusercontent.com/62663286/208293476-fecd01b4-915a-4323-9d61-fef41d4a51df.png)

Here is the terminal picture:

![Screenshot from 2022-12-18 12-33-40](https://user-images.githubusercontent.com/62663286/208293521-4fa275c7-5595-4cae-9c7c-804ae15338df.png)

As you can see, it warns the user about the divisibility and asks if the user wants to continue (0) or not (1). If not continuing (1) is selected, it asks to type the order length again and if it warns when the user manually typed the order, it asks to manually type it again.

### Image sizes

Images used in this readme are really small and simple, but with this program you can also create massive images like for example 40000x40000 pixels so the only limit is your image viewer software's capabilities.

### Bitmap file format

Bitmap files tend to take a lot of space but that's not a problem because you can easily convert bitmap files to png files (and other file formats of course)

### Originality

There are many random pixel image generators out there but none or very few (haven't found any) have the opportunity to create images by color (or black & white) order, which is the greatest and most fun thing in this program.

