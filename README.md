# Baybayin and Latin Binary Images in .mat Format
For discriminating Latin/Roman alphabet from Baybayin script in character recognition.

## Collection of Baybayin Characters
We have gathered some 9000+ Baybayin character images from https://www.kaggle.com/jamesnogra/baybayn-baybayin-handwritten-images. We additionally collected 8000+ images more using a snipping tool to extract each Baybayin character image from several Baybayin related websites. The links for some of these images can be found in URL_Links_with_Baybayin_Images.pdf. We have fixed the data set into 1000 images per character and is formatted as below.

If you have some questions regarding the data set we provide, just email me at rbpino@up.edu.ph. You can check the full paper here: https://peerj.com/articles/cs-360/ where we used the provided dataset.

## Content
The datasets are in MATLAB format and contains binary images of Latin and Baybayin characters and 4 character symbols of Baybayin diacritics.

Each character image is strictly center-fitted with a size 56x56 pixels.

Each character in both considered scripts (including Baybayin diacritics) has a clustered preview photo.

A total of 17,000 images for Baybayin (1000 per character), 18,200 images for Latin (700 per character), and 2000 images for Baybayin diacritics (500 per symbol).

## Main Files Attached

• <b> Baybayin.zip </b> - contains a `Baybayin.mat` file that is in struct format comprising names of the respective character.

• <b> Baybayin Diacritics.zip </b>- contains a `Baybayin_Diacritics.mat` file that is in struct format comprising names of the respective symbol.

• <b> Latin.zip </b> - contains a `Latin.mat` file that is in struct format

• <b> URL_Links_with_Baybayin_Images.pdf </b> - webpages of some Baybayin images that we used are can be found in this pdf file.

• <b> CSV Datafiles.zip </b> - containts CSV datafiles of Baybayin, its diacritics, and Latin character binary images. This file is also deposited to allow for a wider compatibility of the dataset to other programming languages.

• <b> Data Guide Scripts.zip </b> - contains MATLAB codes/functions that are used to reconstruct and validate each image data. 

    ○ Normalization codes:
    
      ► feature_extract_algorithm.m - this is the mother code to execute the feature extraction process of a raw Baybayin character, starting from binarization to extraction of its feature vector.
      ► kmeans_mod.m - this is a subfunction from the feature_extract_algorithm.m for clustering a grayscaled image into 2 intensities intended for image binarization.
      ► c2bw.m - this is a subfunction from the feature_extract_algorithm.m for converting the input raw image into binary image using the modified kmeans function.
      ► feature_vector_extractor.m - this is a subfunction from the feature_extract_algorithm.m that outputs the 1x3136 feature vector array of the input square matrix.
      
    ○ Sample variable and images:
    
      ► Baybayin_A.mat - contains the 1,000 reconstructed images of Baybayin character A
      ► Da_noisy.PNG - noisy image of a Baybayin character Da
      ► EI_noisy.PNG - noisy image of a Baybayin character E/I
      ► Ga_noisy.PNG - noisy image of a Baybayin character Ga
      ► Na_noisy.PNG - noisy image of a Baybayin character Na
      
    ○ Model generators:
    
      ► BINARY - these functions generate binary classifiers for Script classification (Latin and Baybayin), Baybayin diacritics categorization, and binary classifiers for confusive Baybayin characters.
          ☼ data_trainingtesting_binary_KNN.m - generates KNN binary models. 
          ☼ data_trainingtesting_binary_SVM.m - generates SVM binary models.

      ► MULTICLASS - these functions generate multiclass classifiers in recognizing the 17 Baybayin characters.
          ☼ data_traintest3_multiclass_17classes_revisedKNN.m - generates KNN multiclass models.
          ☼ data_traintest3_multiclass_17classes_revisedSVM.m - generates SVM multiclass models.

    ○ Headless run:
    
      ► character_view - use to view a single character image from the compiled dataset.
      ► whole_data_view - use to view a clustered dataset.



## Acknowledgments
Latin characters and Baybayin diacritic images are taken from https://www.kaggle.com/gregvial/comnist/data and https://www.kaggle.com/xainano/handwrittenmathsymbols/data. The images they provided are formatted as mentioned above.

## Inspiration
These datasets are part of the ongoing restoration of the Baybayin script in the Philippines. Others may use some of these for Baybayin or Latin script related researches.
