# Text_Scanner

Project Description

This code uses the functions provided by OpenCV to create a simple scanner. It finds the contours in an image and the biggest contour it find it assumes to be the text image to be scanned. It warps that sub image into a flat rectangular shape and uses adoptive threshold to remove blemishes or other noise to give us only the text part of the image. There are a few limitations to the scanner like assuming that the largest shape (or contour) in the image is the text part and assuming that the text has no images.

Rubic Points Specified

Loops, Functions, I/O

1.The project demonstrates an understanding of C++ functions and control structures .:: The program uses multiple loops and if statements to control the flow of the code.

2.The project reads data from the file and process the data, or the program writes the data to a file .:: the program reads data from an image and writes data to another image after processing it.

3.The project accepts user input and processes the input .:: the program takes as input the name of the image it has to scan from within the images folder and uses it to read the specified image.

Object Oriented Programming

4.Overloaded functions allow the same function to operate on different parameters .:: the function _distance can operate on both two Point variables and 4 coordinates.

Memory Management

5.The project makes use of references in function declaration.:: resizeToHeight, fourPointTransform, preProcess are functions that use pass-by-reference.

How to Run

1)Clone the repository

2)move into the repository

3)clone the openCV repository into it (you can use command :: git clone git@github.com:opencv/opencv.git opencv/)

4)mkdir -p build && cd build

5)cmake ../opencv (assumong that the name of the folder in which the open cv code has been cloned is called opencv)

6)make -j4  

7)cd ..

8)cmake .

9)make

10)./scanner

the program will ask the name of the file which you want to run. The image file to run must be placed within the images folder and full name (with extension) must be used. Currently I have kept a few sample files in there.
below attached is a screenshot of the program being run

![WhatsApp Image 2022-09-10 at 11 39 15 PM](https://user-images.githubusercontent.com/51983729/189496320-ae6b802a-39ac-4e1c-8f1e-89ddb3237c89.jpeg)

the scanned image will be stored in the working directory.

![WhatsApp Image 2022-09-10 at 11 53 28 PM](https://user-images.githubusercontent.com/51983729/189496756-33372130-03aa-4f56-b275-4f61cd0bf733.jpeg)

