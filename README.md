# Computer-vision-color-detection-project
1- Purpose: The script aims to detect and segment specific colors in an image using OpenCV and Python.

2- Image Stack Functionality: The stackImages function is defined to concatenate multiple images into a single one for visualization purposes.

3- Trackbars for Adjustments: Six trackbars are created for adjusting the minimum and maximum values of hue, saturation, and value (HSV) channels.

4- Image Loading: An image of a Tesla Model Y (named "tesla-model-y-long-range-dual-motor-uhCWvzsDrM.jpg") is loaded into the script.

5- Colorspace Conversion: The loaded image is converted from the BGR color space to the HSV color space using cv2.cvtColor.

6- Trackbar Positions: Trackbar positions are retrieved to determine the HSV thresholds for color segmentation.

7- Thresholding: The lower and upper HSV thresholds are defined based on the trackbar positions.

8- Mask Creation: A mask is created using cv2.inRange to identify pixels within the specified HSV range.

9- Bitwise AND Operation: The original image is bitwise ANDed with the mask to obtain the color-detected result.

10- Convert Mask to 3-channel: The mask is converted to a 3-channel image for stacking with other images.

11- Image Stacking: The original image, HSV image, mask, and color-detected result are stacked vertically for display using the stackImages function.

12- Display: The stacked image is displayed in a window named "Stacked Images".

13- Loop: The script continuously updates the displayed image based on trackbar adjustments until the user presses 'q' to quit.

14- Cleanup: Upon quitting the loop, all OpenCV windows are destroyed using cv2.destroyAllWindows.


![Screenshot (147)](https://github.com/Bisma-Shafiq/computer-vision-color-detection-project/assets/148833585/db3877d3-0e6d-41aa-9d67-28e7e43c6d80)
