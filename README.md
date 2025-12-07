# real-time-image-processing

We use the cv2 library to capture the frames to continuously display the frames and even to plot the frames.

We use the function VideoCapture() which is a part of cv2 library and is used to capture frames inside the function - we pass the value 0 if we are using inbuilt camera or 1 2 3 depending in which port you connect your external camera to, in most cases 1 will work. 



## Cropping and flipping

Cropping a video window is similar to cropping a plotted image, like we used slicing to crop a plotted image we can similarly use slicing to crop a video window. 

crop = img [ : , : , : ]                 #[horizontal, vertical, channel]

To flip an image what we mean is to flip the image that is shown in the window. To flip an image, we will use a function known as flip() flip takes 2 arguments: 1 the image and second whether to flip the image horizontally or vertically. 

img = cv2.flip(img , 0) # 0 means vertical flip 

img = cv2.flip(img , 1)      # 1 means horizontal flip



## Frame extraction and HSV

HSV stands for Hue, Saturation and Value. 

Hue defines the main dominating colour
Saturation defines how bright the colours are in the video 
Value will tell us basically how dark the colour is in darkness
