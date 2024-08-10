# Fashion Product Image Generation and Pricing Using GANs

This repository contains a research project that explores the application of Generative Adversarial Networks (GANs) in generating and pricing novel wristwatch designs using the Fashion Product Images Dataset from Kaggle. This project aims to automate the creation and pricing of new fashion products, with a particular focus on wristwatches, by leveraging AI-driven image generation techniques.

## Project Overview

E-commerce has revolutionized the way consumers purchase fashion items, especially during the pandemic when online shopping surged. The fashion industry, however, constantly seeks innovation in design and pricing to stay competitive. This project addresses this need by exploring how AI can be used to generate new fashion product designs, specifically wristwatches, and assign them prices based on specific attributes.

## Objectives

Image Processing and Preprocessing:
Extract wristwatch images from a diverse dataset of e-commerce fashion products.
Perform comprehensive preprocessing, including color conversion, resizing, and normalization, to prepare the images for GAN training.
Image Generation:
Train a Generative Adversarial Network (GAN) on the extracted wristwatch images to create new, realistic designs.
Evaluate the quality of the generated images using metrics like Fréchet Inception Distance (FID), Inception Score (IS), and Structural Similarity Index (SSIM).
Pricing Model:
Develop a color-based pricing system that assigns prices to the generated wristwatch designs based on dominant color intensities.
Utilize the colorThief library to categorize wristwatches into specific price ranges based on their color intensity.


## Dataset

The research utilizes the Fashion Product Images Dataset (Aggarwal, 2019), which contains high-resolution images of various fashion items, including shirts, trousers, bags, t-shirts, socks, wristwatches, shoes, and more. The dataset, with over 44,441 categories, is well-suited for fashion research and applications, particularly in training GAN models for product design.

## Key Dataset Insights

Image Dimensions:
Mean Width: 1397.14 pixels
Mean Height: 1862.87 pixels
Median Width: 1080.0 pixels
Median Height: 1440.0 pixels
Gender Representation:
50.2% for men, 41.6% for women, 1.9% for boys, 1.5% for girls, and 4.8% unisex items.
Wristwatch Data:
The dataset includes 2,542 wristwatch images, all of which were extracted for this research to train the GAN model.

## Methodology

### Data Preprocessing
Image Extraction: Wristwatch images were extracted from the larger dataset and saved in a separate directory.
Preprocessing Steps:
Convert images from BGR to RGB.
Resize all images to 256x256 pixels.
Normalize pixel values to the range of [-1, 1] to ensure stable GAN training.
### GAN Model Training
The GAN was trained on the preprocessed wristwatch images to generate new designs.
Evaluation Metrics:
FID Score: 39.16
Inception Score (IS): 1.00
SSIM: 0.01
### Pricing Strategy
The generated wristwatch designs were assigned prices based on dominant color intensities using the colorThief library.
Intensity > 700: £400 - £500
Intensity > 600: £350 - £400
Intensity ≤ 600: £120 - £350

## Results and Conclusion

The GAN model successfully generated realistic wristwatch designs that closely resemble original images. The pricing model, driven by color intensity, provided a systematic approach to pricing these designs, highlighting its potential application in the fashion industry.

### Key Results
The generated images achieved a Fréchet Inception Distance (FID) score of 39.16, demonstrating a high level of similarity to the real wristwatch images.
The color-based pricing method effectively categorized the wristwatches into different price ranges, making it a promising approach for automating fashion pricing.

## Future Work

This research has laid the groundwork for automated fashion design and pricing. However, several avenues for future work remain:

Improved Computational Resources: Access to more powerful computational resources could enhance the realism and diversity of the generated designs.
Enhanced Pricing Model: Incorporating market research and customer feedback could refine the color-based pricing strategy.
Extension to Other Fashion Items: The techniques used in this research could be applied to other categories of fashion products in the dataset, broadening the scope of the project.

## References

Singh, M., Bajpai, U., V, V. and Prasath, S. (2020) Generation of
fashionable clothes using generative adversarial networks: A preliminary
feasibility study. International Journal of Clothing Science and
Technology, 32(2), pp.177-187.
Creswell, A., White, T., Dumoulin, V., Arulkumaran, K., Sengupta, B. and
Bharath, A.A. (2018) Generative adversarial networks: An overview. IEEE
signal processing magazine, 35(1), pp.53-65.
Sohn, K., Sung, C.E., Koo, G. and Kwon, O. (2020) Artificial intelligence in
the fashion industry: consumer responses to generative adversarial
network (GAN) technology. International Journal of Retail & Distribution
Management, 49(1), pp.61-80.
Kumar, A., Biswas, A. and Sanyal, S. (2018) ecommercegan: A generative
adversarial network for e-commerce. arXiv preprint arXiv:1801.03244.
Peters, T. and Brenner, C. (2020) Conditional adversarial networks for
multimodal photo-realistic point cloud rendering. PFG–Journal of
Photogrammetry, Remote Sensing and Geoinformation Science, 88(3-4),
pp.257-269.
Han, C., Hayashi, H., Rundo, L., Araki, R., Shimoda, W., Muramatsu, S.,
Furukawa, Y., Mauri, G. and Nakayama, H. (2018) GAN-based synthetic
brain MR image generation. 2018 IEEE 15th international symposium on
biomedical imaging (ISBI 2018) (pp. 734-738). IEEE.
Yuan, C. and Moghaddam, M. (2020) Garment design with generative
adversarial networks. arXiv preprint arXiv:2007.10947.
Wikipedia (2023) History of watches. Available online:
https://en.wikipedia.org/wiki/History_of_watches [Accessed 08/07/2023].
Aggarwal, P. (2019) Fashion Product Images Dataset. Available online:
https://www.kaggle.com/datasets/paramaggarwal/fashion-product-
images-dataset [Accessed 08/04/2023].
Goodfellow, I., Pouget-Abadie, J., Mirza, M., Xu, B., Warde-Farley, D.,
Ozair, S., Courville, A. and Bengio, Y. (2020) Generative adversarial
networks. Communications of the ACM, 63(11), pp.139-144.
Singh, S. (2006) Impact of color on marketing. Management
decision, 44(6), pp.783-789.
Funk, D. and Oly Ndubisi, N. (2006) Colour and product choice: a study of
gender roles. Management research news, 29(1/2), pp.41-52.
Great British Watch Company (2014) Global luxury watch and UK watch
repair market. Colin. Available online: https://www.great-british-
watch.co.uk/global-luxury-watch-and-uk-watch-repair-market/ [Accessed
22/07/2023].
Brownlee, J. (2019) How to Evaluate Generative Adversarial Networks.
Available online: https://machinelearningmastery.com/how-to-evaluate-
generative-adversarial-networks/ [Accessed 22/07/2023].
Mathiasen, A. and Hvilshøj, F. (2020) Backpropagating through Fr\'echet
Inception Distance. arXiv preprint arXiv:2009.14075.
Ghojogh, B., Karray, F. and Crowley, M. (2020) Theoretical insights into
the use of structural similarity index in generative models and inferential
autoencoders. In International Conference on Image Analysis and
Recognition (pp. 112-117). Cham: Springer International Publishing.
Salimans, T., Goodfellow, I., Zaremba, W., Cheung, V., Radford, A. and
Chen, X. (2016) Improved techniques for training gans. Advances in
neural information processing systems, 29.
Shmelkov, K., Schmid, C. and Alahari, K. (2018) How good is my GAN?.
In Proceedings of the European conference on computer vision
(ECCV) (pp. 213-229).
Barratt, S. and Sharma, R. (2018) A note on the inception score. arXiv
preprint arXiv:1801.01973.
Nilsson, J. and Akenine-Möller, T. (2020) Understanding ssim. arXiv
preprint arXiv:2006.13846.
