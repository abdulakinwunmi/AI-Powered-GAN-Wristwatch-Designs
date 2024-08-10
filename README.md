# AI-Powered-GAN-Wristwatch-Designs

Fashion Product Image Generation and Pricing Using GANs

This repository contains a research project that explores the application of Generative Adversarial Networks (GANs) in generating and pricing novel wristwatch designs using the Fashion Product Images Dataset from Kaggle. This project aims to automate the creation and pricing of new fashion products, with a particular focus on wristwatches, by leveraging AI-driven image generation techniques.

Project Overview

E-commerce has revolutionized the way consumers purchase fashion items, especially during the pandemic when online shopping surged. The fashion industry, however, constantly seeks innovation in design and pricing to stay competitive. This project addresses this need by exploring how AI can be used to generate new fashion product designs, specifically wristwatches, and assign them prices based on specific attributes.

Objectives
Image Processing and Preprocessing:
Extract wristwatch images from a diverse dataset of e-commerce fashion products.
Perform comprehensive preprocessing, including color conversion, resizing, and normalization, to prepare the images for GAN training.
Image Generation:
Train a Generative Adversarial Network (GAN) on the extracted wristwatch images to create new, realistic designs.
Evaluate the quality of the generated images using metrics like Fréchet Inception Distance (FID), Inception Score (IS), and Structural Similarity Index (SSIM).
Pricing Model:
Develop a color-based pricing system that assigns prices to the generated wristwatch designs based on dominant color intensities.
Utilize the colorThief library to categorize wristwatches into specific price ranges based on their color intensity.
Dataset

The research utilizes the Fashion Product Images Dataset (Aggarwal, 2019), which contains high-resolution images of various fashion items, including shirts, trousers, bags, t-shirts, socks, wristwatches, shoes, and more. The dataset, with over 44,441 categories, is well-suited for fashion research and applications, particularly in training GAN models for product design.

Key Dataset Insights
Image Dimensions:
Mean Width: 1397.14 pixels
Mean Height: 1862.87 pixels
Median Width: 1080.0 pixels
Median Height: 1440.0 pixels
Gender Representation:
50.2% for men, 41.6% for women, 1.9% for boys, 1.5% for girls, and 4.8% unisex items.
Wristwatch Data:
The dataset includes 2,542 wristwatch images, all of which were extracted for this research to train the GAN model.
Methodology

Data Preprocessing
Image Extraction: Wristwatch images were extracted from the larger dataset and saved in a separate directory.
Preprocessing Steps:
Convert images from BGR to RGB.
Resize all images to 256x256 pixels.
Normalize pixel values to the range of [-1, 1] to ensure stable GAN training.
GAN Model Training
The GAN was trained on the preprocessed wristwatch images to generate new designs.
Evaluation Metrics:
FID Score: 39.16
Inception Score (IS): 1.00
SSIM: 0.01
Pricing Strategy
The generated wristwatch designs were assigned prices based on dominant color intensities using the colorThief library.
Intensity > 700: £400 - £500
Intensity > 600: £350 - £400
Intensity ≤ 600: £120 - £350
Results and Conclusion

The GAN model successfully generated realistic wristwatch designs that closely resemble original images. The pricing model, driven by color intensity, provided a systematic approach to pricing these designs, highlighting its potential application in the fashion industry.

Key Results
The generated images achieved a Fréchet Inception Distance (FID) score of 39.16, demonstrating a high level of similarity to the real wristwatch images.
The color-based pricing method effectively categorized the wristwatches into different price ranges, making it a promising approach for automating fashion pricing.
Future Work

This research has laid the groundwork for automated fashion design and pricing. However, several avenues for future work remain:

Improved Computational Resources: Access to more powerful computational resources could enhance the realism and diversity of the generated designs.
Enhanced Pricing Model: Incorporating market research and customer feedback could refine the color-based pricing strategy.
Extension to Other Fashion Items: The techniques used in this research could be applied to other categories of fashion products in the dataset, broadening the scope of the project.
