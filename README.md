# Brief introduction
I do images pixels conversion from RGB to gray scales
All images are stored at src/ directory which I specifiec at program
It can process any size of images only if you have enough big hard drives
Just store the images into src/, this frame work will process them

I implemented a frame with CUDA programming model with multiple GPU devices in ace-tesla.egr.vcu.edu server,
I employ all the 8 GPUs( 2 GeForce GTX TITAN X, 2 Tesla C2070, and 4 Tesla C2050 ) to process image pixels 
In each GPU device, I also divide the data into 4 streams

# Some problems
This server is not solely available for me, sometimes other user will consume too much memory of 2 GeForce GPUs 
This will cause the break down of my program 

# Create folder to store the source color image and target grayscale images
To make sure the program could run, we should create three folders in project directory:

src/ : store the colored images

cpu_tar/ : store the grayscale images which are processed by CPU

gpu_tar/ : store the grayscale images which are processed by GPU

put the images into src/ directory

	make

	sh run

program will work


