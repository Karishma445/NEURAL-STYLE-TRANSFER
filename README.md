# NEURAL-STYLE-TRANSFER

"Company"=CODTECH IT SOLUTIONS

"Name"=D.Karishma

"Intern Id"=CT06DZ2134

"Domain"=Artificial Intelligence

"Duration"=6 weeks

"Mentor"=Neela Santoosh

Neural Style Transfer – Project Description
Introduction
Neural Style Transfer (NST) is an advanced computer vision technique that blends two images — a content image and a style image — to produce a new image that preserves the content of the first while adopting the artistic style of the second. This project implements NST using the PyTorch deep learning framework, following the optimization-based approach first introduced by Gatys et al. in their groundbreaking 2015 paper “A Neural Algorithm of Artistic Style.”

Objective
The main goal of this project is to create a Python-based script or Jupyter Notebook that allows users to apply artistic styles to photographs. By combining the semantic content of one image (such as a landscape or portrait) with the color, texture, and brushstroke patterns of a style image (such as a famous painting), we can produce visually stunning results that resemble human-made art.

Methodology

Model Selection
This implementation uses a pre-trained VGG19 convolutional neural network from the torchvision.models library. VGG19 is trained on ImageNet, which ensures it has learned rich feature representations that can be repurposed for style transfer tasks.

Feature Extraction
The network’s intermediate layer outputs are used to represent both content and style.

Content Features: Captured from deeper layers that encode high-level image structures.

Style Features: Represented using Gram matrices, which measure the correlations between filter responses, capturing texture and color distribution.

Loss Functions

Content Loss: Measures the difference between the content features of the generated image and the original content image.

Style Loss: Measures the difference between the style features (Gram matrices) of the generated image and the style image.
These losses are combined with weighting factors to balance between preserving structure and applying style.

Optimization
The generated image starts as a copy of the content image (or random noise) and is iteratively updated to minimize the combined loss using the L-BFGS optimizer. This process gradually reshapes the image so that it matches both the style and content constraints.

Implementation Details

The script is configurable via command-line arguments for paths, output size, number of optimization steps, and loss weights.

Images are resized to a manageable size (default 512×512) to balance quality and computational time.

The process works on CPU and GPU, with GPU significantly accelerating the optimization.

The script can be run in Google Colab for free GPU access.

Applications

Art Generation: Transform personal photos into artworks inspired by famous paintings.

Content Creation: Enhance social media, advertising, and marketing visuals.

Education: Demonstrates the power of convolutional neural networks for feature representation.

Conclusion
This project successfully demonstrates how deep learning can be applied to creative domains by merging art and technology. By leveraging a pre-trained CNN for feature extraction and iterative optimization, the system produces compelling stylized images that mimic the aesthetics of the chosen style image while maintaining the structure of the content image. The resulting script is flexible, reproducible, and ready for extension into real-time applications using faster feed-forward networks.

<img width="288" height="216" alt="Image" src="https://github.com/user-attachments/assets/e6553779-483c-4eeb-b692-64d5d9100830" />



