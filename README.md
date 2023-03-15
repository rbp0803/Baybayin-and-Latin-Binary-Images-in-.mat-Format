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

## Acknowledgments
Latin characters and Baybayin diacritic images are taken from https://www.kaggle.com/gregvial/comnist/data and https://www.kaggle.com/xainano/handwrittenmathsymbols/data. The images they provided are formatted as mentioned above.

## Inspiration
These datasets are part of the ongoing restoration of the Baybayin script in the Philippines. Others may use some of these for Baybayin or Latin script related researches.
