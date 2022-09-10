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


