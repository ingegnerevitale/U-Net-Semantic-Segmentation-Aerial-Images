# A U-Net model for the automatic Segmentation of aerial images using Dubai’s satellite imagery dataset

## Abstract

For different purposes ,in recent years, deep learning methods have been successfully applied to aerial images. Often, this methodology is very useful for emergency situations that requires decision support systems capable to provide early warning information on critical events and, at the same time, capable to suggest intervention measures in a post disaster scenario. Due to the difficulty in preparing sufficient training samples constrains, producing a deep learning network model with strong generalization is very important. This project was developed by the authors to map buildings that fall into landslide risk areas. The methodology consist in a deep learning approach based on the U-Net model. The U-Net model is trained and validate using the Dubai's Satellite Imagery Dataset. In order to artificially increase the amount of data and avoid overfitting, a data augmentation process was carried out on the training and validation set. In this project the transferability of the baseline model results can be tested in different contexts. The results show that, using this model, a  segmentation of aerial images with a certain level of accuracy can be carried out. 

## Note
A part of source code reported in this project derived from the Amirhossein Heydarian project “U-Net for Semantic Segmentation on Unbalanced Aerial Imagery” available on [Github](https://github.com/amirhosseinh77/UNet-AerialSegmentation).

## Dataset
The training and validation dataset is “Semantic segmentation of aerial imagery”, an open access dataset which [Humans in the Loop](https://humansintheloop.org/) has published for a joint project with the [Mohammed Bin Rashid Space Center](https://www.mbrsc.ae/) in Dubai, the UAE. The dataset contains  72 high resolution satellite images of Dubai with the correspondent semantic segmentation masks. Each satellite image is segmented into 6 classes, including water, land, road, building, vegetation, and unlabeled. The images were segmented by the trainees of the Roia Foundation in Syria. The training and validation sample are respectively of 65 images and 7 images.

## Semantic Annotation
The images are densely labeled and contain the following 6 classes:

![classes_rgb](https://user-images.githubusercontent.com/105599513/176649091-66c6fecc-53af-4e3c-bcfd-0a947e980574.png)

## Sample Images & Masks

![masks](https://user-images.githubusercontent.com/105599513/176650568-11d6232f-7f13-4748-ac97-78f03f741552.png)

## Data augmentation
Data augmentation is done by the following techniques:
- Random Cropping
- Horizontal Flipping
- Vertical Flipping
- Rotation
- Gaussian noise and filtering  operations

## Training and validation results

![metrics graph](https://user-images.githubusercontent.com/105599513/176652538-0db263be-7350-45df-a7fb-83d67d794814.jpg)

## License
This project is released under [GNU General Public License version 3](https://www.gnu.org/licenses/gpl-3.0.html)

## Project Application To Emergencies Scenarios.
Natural disasters have a significant impact on urban areas, resulting in loss of lives and urban services. Using satellite and aerial imagery, the rapid and automatic assessment of at-risk located buildings from can improve the overall disaster management system of urban areas. To do this, the definition, and the implementation of models with strong generalization, is very important. Starting from these assumptions, the authors proposed a deep learning approach based on the U-Net model to map buildings that fall into mapped landslide risk areas. The U-Net model is trained and validated using the Dubai’s Satellite Imagery Dataset. The transferability of the model results are tested in three different urban areas within Calabria Region, Southern Italy, using natural color orthoimages and multi-source GIS data. The results show that the proposed methodology can detect and predict buildings that fall into landslide risk zones, with an appreciable transferability capability. During the prevention phase of emergency planning, this tool can support decision-makers and planners with the rapid identification of buildings located within risk areas, and during the post event phase, by assessing urban system conditions after a hazard occurs.

[Paper Link] (https://www.mdpi.com/2072-4292/14/17/4279)
