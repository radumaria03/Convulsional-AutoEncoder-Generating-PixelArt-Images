# Convulsional-AutoEncoder-Generating-PixelArt-Images

# PyTorch Model for reconstructing Pixel Art Images

**The Model was trained using the Tiny Hero dataset - 3648 images with Pixel Art characters**
 * Image size: 64*64px
 * Colored images -> Image shape: `(3, 64, 64)`


<img width="495" height="112" alt="dataset" src="https://github.com/user-attachments/assets/8b067376-8af3-4f2f-a519-a3d985ca0fcd" />


# Experimenting and gradually improving the model
**Model 0**
 * using a Convulsionaal AutoEncoder
 * Loss Function: `MLELoss()`
 * No *Data Augmentation*


<img width="500" height="311" alt="5epochs" src="https://github.com/user-attachments/assets/f09a5a85-87d8-43ee-8128-496b92b42964" />


**50 Epochs Results**

<img width="500" height="311" alt="5epochs" src="https://github.com/user-attachments/assets/f28b1688-687e-4fb6-a995-7881f95200c8" />

**Training Time** (Google Colab Free Plan)

<img width="645" height="186" alt="training time" src="https://github.com/user-attachments/assets/14cfc8ba-3f52-4cec-b809-b5fc463c18ce" />


**Improving Model 0**
 * changing from `MLELoss()` to `SmoothL1Loss()`
 * adding Data Augmentation using `transforms`
 * training the model for longer


<img width="635" height="322" alt="improvments" src="https://github.com/user-attachments/assets/1b403a3e-0ff0-4c02-a50c-19af2e1c87fe" />


**Sobel Filter for Edge Detection**
 * since we are working with pixel art characters, edge detection worked great for the model


<img width="656" height="380" alt="filter" src="https://github.com/user-attachments/assets/38fec69d-9584-45bd-ae36-19d5ea883128" />
<img width="653" height="397" alt="filter2" src="https://github.com/user-attachments/assets/15e61230-6a0a-4968-b7cf-bb4b0157d459" />




