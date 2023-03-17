To start code, you need to give path of image manually.

I used NCC to calculate similarities

I used meanStdev to calculate mean and standard deviations.

I used calculateHistogram to calculate and show histogram of images.

Color transfer process is in colorTransfer function. It returns color transferred image.

Part 2 is in part2 function. It calculate NCC for small rectangles and calls color transfer function for
this rectangles. It returns color transferred image.

If you want to run part2 instead of part1, simply comment the line with call for colorTransfer function
and uncomment the line with call for part2 function.

cv2_imshow() methods are just visualize in Google Colab, cv2.imwrite() methods are get output image as .png file.

You also need to give path manually to cv2.imwrite() and calculateHistogram methods.

