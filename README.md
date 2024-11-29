# blood_group_identification

7. How to save an image using opencv

    -> imwrite()

        -> used to store the images used in our project with different names for future purpose.

    syntax:

    cv2.imwrite(imagename,image_source)

import cv2

img = cv2.imread('blood cell.jpg',cv2.IMREAD_GRAYSCALE)

imagename = 'grayscale_converted_image.jpg'

cv2.imwrite(imagename,img)

# img = cv2.imread('grayscale_converted_image.jpg')

# cv2.imshow('output',img)

cv2.waitKey(0)

cv2.destroyAllWindows()

8. How to resize the images which we read.

    -> most of the time, we will not get the perfect size of the image, sometimes it will be large or too small. So, we need to

    re-size the image to common size.

    -> resize()

        -> used to re-size the images to a common size.

    syntax:

    cv2.resize(source,dsize,destination,fx,fy,interpolation)

    source -> image which we have read

    dsize -> size of the output iamge

    destination -> the output image to be saved once again (work like imwrite())

                -> optional

    fx - scale factor on horizontal axis

    fy - scale factor on vertical axis

    interpolation - automated sizing

        -> INTER_AREA

            -> when we are going to use a image as shrinked one

        -> INTER_CUBIC

            -> slowest resizing option

        -> INTER_LINEAR

            -> when we are going to use a image as zoomed one

        -> optional

    1. half image condition

        -> dsize = (0,0)

        -> fx > 0

        -> fy > 0

18:03has context menu  """
