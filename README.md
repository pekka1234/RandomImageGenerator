# RandomImageGenerator

## What is it?

Random Image Generator is a command line tool written in C++ to create bitmap images randomly or by input. 

Here are some example images that are generated using this program:

Note: some images are screenshots of the actual images because they are so small.

![Screenshot from 2022-12-05 18-23-51](https://user-images.githubusercontent.com/62663286/208254655-1d2ab30b-c047-4c88-b0c2-49a120879f44.png)
![Screenshot from 2022-12-17 19-45-43](https://user-images.githubusercontent.com/62663286/208254662-cc479d23-a324-40c5-b949-a4e9916120ad.png)
![cc](https://user-images.githubusercontent.com/62663286/208254675-4196c62d-4c54-4edb-bb4a-06fd5b8967ab.png)
![Screenshot from 2022-12-17 19-49-38](https://user-images.githubusercontent.com/62663286/208254792-b40f0fe7-adfd-44e4-8b33-4dc6d49f8106.png)

## How to use it?

Here is an image of the command line after an image is created:

![Screenshot from 2022-12-17 19-55-19](https://user-images.githubusercontent.com/62663286/208255073-8e22925d-1e5e-457e-a299-f32967cbbd66.png)

Here is the above image creation process in steps:

Note: When values are put in the terminal, no spaces are allowed

1. Selecting if image will be black & white (0) or color image (1). In image creation above, black & white (0) was selected.

2. Inserting image' width and height in pixels. In image creation above, 500 was selected to be the width and height.

3. Deciding if image is generated by manually typed order (what orders mean, is explained later on), or randomly (random option includes randomizing color for eachpixel seperately and generating random order by given order length). In image creation above, order 1010100000000000111111111010101 was selected.

4. Entering file's name

Note: Steps above are for black and white images images generated by manually typed order and for diferent images, the creation steps are diferent and for those images that are not explained above will be explained later

### How black & white image's order work?

Note: Orders are most important and fun thing is this progrma because the images can look quite interesting.

In this program (when black & white images are used), orders mean sequences of blacks and whites, for example: black,white,white is an order and if that order is put to a 20x20 image, the image would look like this:

![Screenshot from 2022-12-18 10-49-04](https://user-images.githubusercontent.com/62663286/208289288-fb5b5f0a-8c74-4328-b713-f969d3a7781a.png)

In above image you can see that the pixels (starting from up left) are black,white,white,black,white,white... and so on just like the order was (black,white,white) so the orders are just sequences of blacks and white that will fill the image. Orders are inserted to the program in a way that black = 1 and white = 0 so the above image was created using order 100.

Here is the termianl after the above image was created:

![Screenshot from 2022-12-18 10-57-32](https://user-images.githubusercontent.com/62663286/208289594-1bc3373b-a847-47cf-bd86-7a587e29b78e.png)
