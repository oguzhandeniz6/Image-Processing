def gaussianPyramid -> Takes image and returns a list that contains gaussian pyramid steps

def laplacianPyramid -> Takes gaussian pyramid list and returns a list that contains laplacian pyramid steps

def prepareMask -> To create custom, rectangular mask automatically.

Main input image -> apple, crosswalk, supra... (image to be applied on)
Other input image -> orange, beatles, gtr... (partially used image)

layerCount -> Number of pyramid levels

You need to copy the mask part according to your need.

apple-orange
#############################################################
mask = prepareMask(main.shape, 0, main.shape[0], main.shape[0] // 2, main.shape[0])
#############################################################
# this will create half black half white mask image


mona lisa
#############################################################
other[125:150,180:275] = other[150:175,175:270]
mask = prepareMask(main.shape, 125, 150, 180, 275)
#############################################################
# this will create a white part in mona lisa's forehead


supragtr
#############################################################
other = cv2.resize(other, (main.shape[1], main.shape[0]))
mask = prepareMask(main.shape, 385, 820, 200, 1180)
#############################################################
# this will create a rectangular mask for half of the car



iloveyoupaa
#############################################################
mask = prepareMask(main.shape, 65, 190, 60, 350)
#############################################################
# this will create a rectangular mask for middle of image


beatles
#############################################################
mask = cv2.imread("/content/sample_data/beatlesmask.jpg")
#############################################################
# this will read the mask as input, i drew it by hand


I explained other parts as comment line in code, part by part.