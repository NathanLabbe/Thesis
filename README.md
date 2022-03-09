# Detecting illegal gold mining sites in the Amazon forest Using Deep Learning to Classify Satellites Images
This Master Thesis is part of my MSc degree at KTH Royal Institue of Technology in Stockholm, Sweden
The [publish paper](https://www.diva-portal.org/smash/record.jsf?pid=diva2%3A1633659&dswid=-1136) can be found on Diva

### Abstract
Illegal gold mining in the Amazon forest has increased dramatically since 2005 
with the rise in the price of gold. The use of chemicals such as mercury, which 
facilitate the gold extraction, increases the toxicity of the soil and can enter the food
chain, leading to health problems for the inhabitants, and causes the environmental
scourge we know today. In addition, the massive increase in these activities favours
deforestation and impacts on protected areas such as indigenous areas and natural
reserves. Organisations and governments from Peru, Brazil and French Guyana in
particular, are trying to regulate these activities, but the area to cover being very large,
by the time illegal exploitation is detected it is often too late to react.
The idea of this thesis is to evaluate whether it is possible to automate the task of
detecting these illegal gold mines using open satellite images and deep learning. In
order to answer this question, this report includes the creation of new datasets, as
well as the evaluation of two techniques which are object detection using RetinaNet
and semantic segmentation using U­Net. The influence of image spectral bands is also
studied in this thesis. The numerous trained models are all evaluated using the Dice
Coefficient and Intersection over Union metrics, and each comparison is supported by
the statistical sign­test.
The report shows the superiority of the segmentation model for the binary
classification of illegal mines. However, it is suggested to first use RetinaNet to find out
more precisely whether the mine is legal or illegal, and then to use U­Net if the mine is
illegal in order to make a more precise segmentation. It also shows and illustrates
the importance of using the right image spectral bands which greatly increases the
accuracy of the models.

## Conclusion 
The work show better results on using false colour images, since select specific spectral bands can highlight the object we want to detect as shown in the following pictures.
![True vs False](https://github.com/NathanLabbe/Thesis/blob/main/False%20Colour%20vs%20True%20Colour.png?raw=true)

The paper propose a combination of a Multiclass Object Detection model in order to search for illegal mines, and then a Binary Semantic Segmentation model if any illegal mines have been found. The architecture is pictured in the following image.
![Combination](https://github.com/NathanLabbe/Thesis/blob/main/Model%20Combination.png?raw=true)

## Author
* [Nathan Labbe](https://github.com/NathanLabbe)
