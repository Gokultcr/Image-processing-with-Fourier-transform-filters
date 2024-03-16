# Image Processing with Fourier Transform Filters

This script performs various image processing tasks using Fourier Transform filters. 

### Step 1: Import Libraries

Importing necessary libraries such as `cv2` for computer vision operations, `numpy` for numerical computations, `matplotlib.pyplot` for plotting, and `math` for mathematical functions.

### Step 2: Load and Display Images

Two images are loaded using `cv2.imread` function. The first image is loaded grayscale. These images are then displayed using `matplotlib.pyplot`.

### Step 3: Fourier Transform

The images are transformed into the frequency domain using Fourier Transform (`np.fft.fft2`). The zero frequency component is shifted to the center (`np.fft.fftshift`). Then, the inverse operations are performed to bring back the image to its original position (`np.fft.ifftshift`, `np.fft.ifft2`).

### Step 4: Plotting Spectrums

Here, plots various spectrums of the images including the original spectrum, centered spectrum, and decentralized spectrum using `matplotlib.pyplot`.

### Step 5: Implementing Filters

Several types of filters are implemented:
- Ideal Low-pass and High-pass Filters
- Butterworth Low-pass and High-pass Filters
- Gaussian Low-pass and High-pass Filters

These filters are defined as functions taking parameters such as cutoff frequency (`D0`) and image shape.

### Step 6: Applying Filters

One of the images is chosen, and a low-pass filter is applied to it. The steps include centering the spectrum, applying the filter, and then reversing the operations to obtain the processed image.

### Step 7: Plotting Results

The original image, its spectrum, centered spectrum, multiplied spectrum with the low-pass filter, decentralized spectrum, and the processed image are plotted using `matplotlib.pyplot`.

## Conclusion
This code provides a comprehensive demonstration of image processing techniques using Fourier Transform filters.
