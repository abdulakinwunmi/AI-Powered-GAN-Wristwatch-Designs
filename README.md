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

Aggarwal, P. n.d. Fashion Product Images Dataset. Kaggle. https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset

Kumar, A., Biswas, A. and Sanyal, S., 2018. ecommercegan: A generative adversarial network for e-commerce. arXiv preprint arXiv:1801.03244.

Creswell, A., White, T., Dumoulin, V., Arulkumaran, K., Sengupta, B., & Bharath, A. A. 2018. Generative adversarial networks: An overview. IEEE Signal Processing Magazine, 35(1), 53-65. doi:10.1109/MSP.2017.2765202

Han, C., et al. 2018. GAN-based synthetic brain MR image generation. In 2018 IEEE 15th International Symposium on Biomedical Imaging (ISBI 2018), Washington, DC, USA, (pp. 734-738). doi:10.1109/ISBI.2018.8363678

Singh, M., Bajpai, U., V., V., & Prasath, S. 2020. Generation of fashionable clothes using generative adversarial networks: A preliminary feasibility study. International Journal of Clothing Science and Technology, 32(2), 177-187. https://doi.org/10.1108/IJCST-12-2018-0148

Sohn, K., Sung, C.E., Koo, G., & Kwon, O. 2021. Artificial intelligence in the fashion industry: consumer responses to generative adversarial network (GAN) technology. International Journal of Retail & Distribution Management, 49(1), 61-80. https://doi.org/10.1108/IJRDM-03-2020-0091

Yuan, C. and Moghaddam, M., 2020. Garment design with generative adversarial networks. arXiv preprint arXiv:2007.10947.

Peters, T., & Brenner, C. 2020. Conditional adversarial networks for multimodal photo-realistic point cloud rendering. PFG – Journal of Photogrammetry Remote Sensing and Geoinformation Science, 88(9), 257-269. doi:10.1007/s41064-020-00114-z.

Goodfellow, I., Pouget-Abadie, J., Mirza, M., Xu, B., Warde-Farley, D., Ozair, S., Courville, A., & Bengio, Y. 2020. Generative adversarial networks. Communications of the ACM, 63(11), 139-144. https://doi.org/10.1145/3422622

Brownlee, J. 2022. How to evaluate generative adversarial networks. Machine Learning Mastery. https://machinelearningmastery.com/how-to-evaluate-generative-adversarial-networks/

Mathiasen, A. and Hvilshøj, F., 2020. Backpropagating through Fr\'echet Inception Distance. arXiv preprint arXiv:2009.14075.

Barratt, S. and Sharma, R., 2018. A note on the inception score. arXiv preprint arXiv:1801.01973.

Nilsson, J. and Akenine-Möller, T., 2020. Understanding ssim. arXiv preprint arXiv:2006.13846. 

Salimans, T., Goodfellow, I., Zaremba, W., Cheung, V., Radford, A. and Chen, X., 2016. Improved techniques for training gans. Advances in neural information processing systems, 29.

Shmelkov, K., Schmid, C. and Alahari, K., 2018. How good is my GAN?. In Proceedings of the European conference on computer vision (ECCV) (pp. 213-229).

Ghojogh, B., Karray, F. and Crowley, M., 2020, June. Theoretical insights into the use of structural similarity index in generative models and inferential autoencoders. In International Conference on Image Analysis and Recognition (pp. 112-117). Cham: Springer International Publishing.

Singh, S. 2006. Impact of color on marketing. Management Decision, 44(6), 783-789. https://doi.org/10.1108/00251740610673332

Funk, D. and Oly Ndubisi, N. 2006. Colour and product choice: a study of gender roles. Management Research News, 29(1/2), 41-52. https://doi.org/10.1108/01409170610645439 

History of watches. n.d. Wikipedia, the Free Encyclopedia. Retrieved August 8, 2023, from https://en.wikipedia.org/wiki/History_of_watches

Great British Watch. 2023, March 8. Global luxury watch and UK watch repair market. Retrieved August 8, 2023. https://www.great-british-watch.co.uk/global-luxury-watch-and-uk-watch-repair-market/
