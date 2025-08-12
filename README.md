This project implements a Pix2Pix-style GAN for translating IHC-stained microscopy images into H&E-stained counterparts.
Built in PyTorch, it uses an RGB-to-RGB UNet generator and PatchGAN discriminator to handle high-resolution 1024×1024 image-to-image translation.

Key Features

    Dataset: 190 manually paired IHC → H&E images (slightly misaligned) split into training/validation sets.

    Architecture: UNet-based generator, PatchGAN discriminator.

    Challenges Addressed:

        Slight misalignments between IHC and H&E pairs.

        Color calibration (current outputs are overly pink and low in detail).

    Improvements:

        Alignment-robust loss functions (e.g., perceptual loss, SSIM).

        Architectural tweaks for high-res generation.

        Advanced augmentation strategies.

Tech Stack

    PyTorch

    Python

    GANs / Image-to-Image Translation

    Deep Learning Optimization & Evaluation
