# Underwater Color Correction 

This Python code demonstrates an image dehazing algorithm based on the Dark Channel Prior method. It removes haze and improves visibility in hazy images. The code uses OpenCV, NumPy, SciPy, and the OpenCV ximgproc module.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- SciPy

## Usage

1. Ensure that the required dependencies are installed.
2. Download or clone the repository to your local machine.
3. Place the hazy image you want to dehaze in the same directory as the code file.
4. Update the code to specify the correct filename of the hazy image in the `img=cv2.imread("your_image.png")` line.
5. Run the code.

The dehazed image will be displayed as the output.

## Algorithm Steps

1. Bright Channel Estimation: Computes the bright channel of the hazy image.
2. Channel Intensities Calculation: Determines the intensities of the color channels.
3. Background Subtraction: Subtracts the background of the hazy image.
4. Rectify Brightness: Adjusts the brightness of the image.
5. Atmospheric Light Estimation: Estimates the atmospheric light in the image.
6. Initial Transmission Estimation: Estimates the initial transmission map of the image.
7. Refined Transmission Estimation: Refines the transmission map using guided filtering.
8. Restoration: Restores the image by removing the haze.
9. Histogram Equalization: Enhances the contrast of the restored image.

## References

- Original Paper: "Single Image Haze Removal Using Dark Channel Prior" by Kaiming He, Jian Sun, and Xiaoou Tang.




<h2> Original Image </h2>

![original_image](https://user-images.githubusercontent.com/120055921/213677159-a9eb921a-2169-47e2-858d-052010d1ffc8.jpeg)
<br>
<h2> Final Result</h2> 

![Final_result](https://user-images.githubusercontent.com/120055921/214812005-7d28f402-7fb9-447e-9e18-dae6c1c9ea0e.jpeg)
