# Stop sign and Pedestrian Crossing sign recognition using Template Matching and Image Pyramid

The goal of this project is to detect if there is a STOP sign or a Pedestrian Crossing sign in an image. Two traditional Computer Vision techniques called Template
Matching and Image Pyramid are used to do this. An example of STOP sign and Pedestrian Crossing sign templates is shown

Some quick prototype code to experiment with some old computer vision concepts and get some first time exposure. This code takes a prototype stop sign and Pedestrian crossing sign and creates a 4-level gaussian pyramid out of it by downsampling (read more here: https://en.wikipedia.org/wiki/Pyramid_(image_processing)) then it slides the pyramid one slice at a time over the target image, computing the normalized cross correlation (NCC). The slice with the higher NCC value is determined to be the stop sign.
