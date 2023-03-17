I downloaded both of .py and .ipynb versions of it.

To start code, you need to give path of image manually because there was no file to iterate over names of photos.

I didn't use SSD function in latest version of code, but i didn't delete it.

I used NCC function to calculate differences.

I used alignment function to align RGB channels.

I aligned Green and Red channels TO Blue channel as you stated in pdf.

cv2_imshow() methods are just visualize in Google Colab, cv2.imwrite() methods are get output image as .jpg file.

You also need to give path manually to cv2.imwrite() methods.