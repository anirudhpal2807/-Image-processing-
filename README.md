# -Image-processing-
Basic Introduction to Image processing 
Title: Basic Introduction to Image Processing
Author: Anirudh pal (ECE-IoT), IIIT Nagpur

This script demonstrates the basics of image processing in MATLAB. It includes:

Reading and Displaying a Color Image: The script reads a color image (yellowlily.jpg) and displays it.
Extracting RGB Channels: (Commented code) The red, green, and blue channels of the image can be individually extracted and visualized by setting other channels to zero.
Grayscale Conversion: The color image is converted to grayscale using the built-in rgb2gray function.
Side-by-Side Comparison: The grayscale and original color images are displayed side-by-side using the montage function.
This basic introduction provides a foundational understanding of handling images and manipulating their color channels in MATLAB.

% RGB to Grayscale image ,
clc;
clear all;
close all;
% Reading the data in a variable 
colorimg=imread("yellowlily.jpg");
imshow(colorimg); %print the image 

% Printing out different channels in an Color image (R , G , B)
% just using a variable to store the image and putting values of channels
% to 0 one by one 


 %img_color(:,:,2)=0;
 %img_color(:,:,3)=0;
 %Img_R=img_color;
 %subplot(2,2,1)
 %imshow(Img_R);

 %img_color_2=colorimg;
 %img_color_2(:,:,1)=0;
 %img_color_2(:,:,3)=0;
 %Img_G=img_color_2;
 %subplot(2,2,2)
 %imshow(Img_G);

 %img_color_3=colorimg;
 %img_color_3(:,:,1)=0;
 %img_color_3(:,:,2)=0;
 %Img_B=img_color_3;
 %subplot(2,2,3)
 %imshow(Img_B);

% Conveting an color image into an grayscale image by Using the inbuild
% function rgb2gray

grayImage=rgb2gray(colorimg);
montage({grayImage,colorimg}); % Showing the images side by side
