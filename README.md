trafficSignRecognition
======================

traffic sign recognition based on color classification

This is one research topic under the USC ISI research department. Our final goal is to detect the traffic sign from the
video stream captured by a camera in fron of the car. Currently, our target focus on the speed limit sign.
from German traffic sign dataset.  http://benchmark.ini.rub.de/?section=gtsrb&subsection=news

The whole system is divided into 2 parts. a color classification module and a tracking module. the classifier is used to get
the  ROCs(region of interest) and the tracking module is used to increase the recognition accuracy by using the temporal
information. Our research is still in the first step.

In the color classification module, we want to classfy each pixel as red, or not red in the whole image so that we can 
get ROC(region of interest). Our method is very simple and intuitive. a proposal is here:
https://docs.google.com/document/d/1x8a7xfxbuF9vXX8B-hxFJg8rnh2BRkMaiVl8Qp4OgQM/edit
But classify every pixel could be time consuming. we use several tricks to improve the performance, like image hierarchy
and a strong prior function.




