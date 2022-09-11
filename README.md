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

3)clone the openCV repository into it (you can use command :: git clone git@github.com:opencv/opencv.git opencv/ or in visual studios press ctrl+shift+p to open the command palette and type Git Clone. It will as for the URL to clone from. Use the URL :: https://github.com/opencv/opencv.git. It will then ask where to store the cloned repository. Move inside the Text_Scanner folder and press select repository.)
After cloning it should look like this.

![WhatsApp Image 2022-09-11 at 7 23 37 PM](https://user-images.githubusercontent.com/51983729/189531534-6d33d688-1559-4be6-b331-1ae7e71c02d7.jpeg)


4)mkdir -p build && cd build

5)cmake ../opencv (assumong that the name of the folder in which the open cv code has been cloned is called opencv)


![WhatsApp Image 2022-09-11 at 7 23 37 PM (1)](https://user-images.githubusercontent.com/51983729/189531590-e3ee0638-2a23-4d9d-b2df-de0cd682c418.jpeg)


6)make -j4  

![WhatsApp Image 2022-09-11 at 7 23 37 PM (2)](https://user-images.githubusercontent.com/51983729/189531669-7e40b496-2b1a-44bd-97e5-10f660a16cab.jpeg)


6.5)sudo make install

![WhatsApp Image 2022-09-11 at 7 23 37 PM (3)](https://user-images.githubusercontent.com/51983729/189531725-4d7874ce-7433-425d-865b-54100263d5f6.jpeg)


7)cd ..

8)cmake .

![WhatsApp Image 2022-09-11 at 7 23 37 PM (4)](https://user-images.githubusercontent.com/51983729/189531762-7de4cdf9-0212-4eab-9d7e-0ceb96b788e0.jpeg)


9)make

10)./scanner

![WhatsApp Image 2022-09-11 at 7 23 37 PM (6)](https://user-images.githubusercontent.com/51983729/189531786-9e7434cb-0b25-4f3f-9921-5a85f92ee4d4.jpeg)


the program will ask the name of the file which you want to run. The image file to run must be placed within the images folder and full name (with extension) must be used. Currently I have kept a few sample files in there.
below attached is a screenshot of the program being run

![WhatsApp Image 2022-09-10 at 11 39 15 PM](https://user-images.githubusercontent.com/51983729/189496320-ae6b802a-39ac-4e1c-8f1e-89ddb3237c89.jpeg)

the scanned image will be stored in the working directory.

![WhatsApp Image 2022-09-10 at 11 53 28 PM](https://user-images.githubusercontent.com/51983729/189496756-33372130-03aa-4f56-b275-4f61cd0bf733.jpeg)

