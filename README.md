# Grayscale Converter
> Colored PPM image to grayscale PGM images

## Basic Concept
This is my first project working with **PPM files** and **PGM files**. For this project, I developed a program that produces six different color to black and white conversion using a PPM image file.

This project has two files: 'main.c' and 'image.c'. 
In 'image.c', I used structures for PPM, PGM, as well as pixels. So each of the PPM image (input), has a structure developed through readPPM function which has information like the width, height, rgb numbers using the pixels structure, and more. Then, by using one of the functions (extractRed, extractGreen, extractBlue, computeAverage, computeLightness, computeLuminosity), we then create a structure PGM with grayscale numbers as pixels. After all, we then use the writePGM file to write variables stored in the PGM structure to a new PGM file.

## Installation
To run the program, first download the zip file and extact or clone the repository with the command `git clone https://github.com/namitoyokota/grayscale-converter.git`. Afterwards, direct to the folder in terminal and run the make file with `make` command.

This will produce PGM files for the default PPM file, 'Strawberry.ppm'. In order to add PPM files of your choice, simply drag the PPM file to the directory and open the makefile. In make, change 'Strawbeery.ppm' to the file name of the new PPM file that you imported and change al of the output file names of your choice. 

OR

In order to use your own PPM to create grayscale pictures, move your PPM image to 'BackToThePast' directory and go into makefile. In there, change 'Stawberry.ppm' to the name of your PPM file, and change the output file names to whatever you choose. Then, in terminanl, run makefile with `make`.

## Screenshots
![Before](/Screenshots/Strawberry.png "Before")
![Red](/Screenshots/Strawberry_Red.png "Red")
![Green](/Screenshots/Strawberry_Green.png "Green")
![Blue](/Screenshots/Strawberry_Blue.png "Blue")

## Resources
This project and the algorithm is from <a href="https://www.johndcook.com/blog/2009/08/24/algorithms-convert-color-grayscale/">John Cook</a>
