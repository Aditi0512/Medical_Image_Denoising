#Medical Image Denoising Project
#Introduction
Medical image denoising is a critical component of medical image processing, aimed at improving the accuracy of diagnosis by reducing noise in medical imaging modalities like X-ray, MRI, ultrasound, and CT scans. This project explores traditional and modern denoising techniques to achieve this goal.

#Objective
The goal of this project is to explore and evaluate various denoising methods, including wavelet denoising, total variation denoising, non-local means denoising, median filtering, Gaussian filtering, and denoising using an autoencoder neural network. Performance evaluation is done based on the Peak Signal-to-Noise Ratio (PSNR) metric.

#Literature Survey
In the literature survey, we have reviewed several key papers and techniques related to image denoising, including wavelet-based denoising, total variation denoising, non-local means denoising, median and Gaussian filtering, and deep learning-based denoising methods.

#Methodology
Step 1: Importing Required Libraries
numpy: For numerical computations.
matplotlib.pyplot: For visualization of images and plots.
skimage.io: For reading and writing images.
skimage.restoration: For denoising using various methods.
skimage.metrics: For calculating PSNR.
scipy.ndimage: For applying median and Gaussian filters.
keras.models and keras.layers: For building the autoencoder model.
skimage.transform: For resizing images.
glob: For finding image file paths.
Step 2: Defining Image Paths and Dataset Directory
Set the paths of the input images and the directory containing the dataset.

Step 3: Loading and Preprocessing Input Images
Load and preprocess the input images.

Step 4: Adding Noise to Resized Images
Introduce noise to the resized images for denoising evaluation.

Step 5: Initializing Denoised Image Lists
Create empty lists for storing denoised images obtained using different denoising methods.

Step 6: Building the Autoencoder Model
Define the architecture of the autoencoder using keras.layers and compile the model with an optimizer and loss function.

Step 7: Loading and Preprocessing Images from the Dataset
Retrieve image paths using glob, read, resize, and normalize each image from the dataset.

Step 8: Training the Autoencoder on the Dataset
Fit the autoencoder model to the resized and normalized images from the dataset.

Step 9: Denoising the Resized Images Using Various Methods
Perform denoising using various methods for a specified number of runs and store the denoised images.

Step 10: Apply Different Denoising Methods to the Noisy Images
Apply wavelet denoising, total variation denoising, non-local means denoising, median filtering, Gaussian filtering, and autoencoder denoising to the noisy images.

Step 11: Calculating the PSNR for Each Denoising Method
Compute the PSNR between each resized image and its denoised version using peak_signal_noise_ratio and store the PSNR values.

Step 12: Calculating the Average PSNR Across All Runs
Calculate the average PSNR for each denoising method by averaging the PSNR values across all runs.

Step 13: Visualizing the Results
Display the PSNR values for each iteration and the average PSNR for each denoising method. Plot and display the original, noisy, and denoised images for each iteration and method.

#Conclusion
This project explores various image denoising techniques, comparing their performance in medical image denoising. The evaluation is based on PSNR, aiming to enhance image quality for improved diagnosis in medical imaging and related applications.
