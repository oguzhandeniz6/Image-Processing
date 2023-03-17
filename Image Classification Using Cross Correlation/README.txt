-I used os module to read images from folder automatically.
-readNlist() function reads images in folder and append them to a list.

-I implemented my Normalized Cross Correlation function as NCC.
-find_peak_offset() function finds peak and offset values for one template image and for 
one target image by sliding template image over target image area.

-Since I've worked on Google Colab, I used cv2_imshow() method and 
from google.colab.patches import cv2_imshow module.

-You need to give folder locations to "template_folder_location" and 
"target_folder_location" variables as strings.
-Since I've worked on target folders seperately, you need to give letter to
"target_name" variable. 

-First loop is for target images, second loop is for template images. Tries to match 
every template image for a target image.

-I wrote as comment line but I'd like to mention it here too. While calculating accuracy,
Since there is no True Negative, accuracy = True Positive / All
(All target images are same letter. So if correct, it's True Positive;
 if wrong, it's False Positive)

-It takes about 7~ minutes to classify 30 images (1 target folder).
