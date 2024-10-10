Description
___
In Sub-Saharan Africa, it is estimated that crop diseases and pests can reduce yields by up to 40% annually, with significant impacts on the food security and the economy of the region. This is a major concern, considering that agriculture employs more than 60% of the population and accounts for about 23% of the region's GDP.

Crop diseases are on the rise, exacerbated by climate change and the lack of access to advanced agricultural technologies. Diseases like tomato leaf curl virus and pepper blight have significantly impacted the yields of these essential crops.

The objective of this challenge is to develop robust machine learning models that can accurately predict all diseases present in images of corn, pepper, and tomato crops. Participants are tasked with creating models that can a) generalise well, even when encountering new diseases not seen in the training set, and b) operate efficiently on edge devices such as the entry-level smartphones used by most subsistence farmers in Africa.

By harnessing the power of machine learning, we aim to develop advanced solutions for detecting and identifying multiple diseases in three vital crops: corn, pepper, and tomatoes. The models and solutions developed in this challenge will support accurate and timely disease detection, enhance agricultural productivity and sustainability, and ensure food security for millions of people.

[zindi image](zindi.png)
> [link to the competiton just incase](https://zindi.africa/competitions/ghana-crop-disease-detection-challenge)

Evaluation
___
The error metric for this competition is Mean Average Precision @ Intersection over Union(IoU) threshold -0.5.

Your submission file should look like this:

Image id class confidence ymin xmin ymax xmax

ID_2TZLLT80 Rot 0.5 130 12 340 300

    Image_Id: is the Id assigned to each image. Note, that each image can have more the one object , which translates to more than one bounding box.
    Class: is the particular bounding box classification, i.e. Rot, etc.
    Confidence score: each object detector model gives the confidence score of each bounding box predicted in an image; this value is used to sort the bounding boxes.

Please note additional requirements for submissions under the Explainability and Resource Restrictions sections.


Explainability
___
As part of RAIL's commitment to Responsible AI, all submitted solutions must include explainability components. Participants are required to integrate explainability techniques such as Grad-CAM, LIME, or SHAP. These techniques should provide clear, visual explanations of how the models make their predictions, ensuring transparency and fostering trust in the AI solutions.

Please note that this is a requirement for winning in this challenge.


Resource Restrictions
___
Your solutions for this challenge must be able to function in a resource-limited setting i.e. it should run on a low-resource smartphone. As such, we are imposing the following restrictions on resources:

    T4 GPU, maximum 9h training, maximum 3h inference
    Model frameworks must be appropriate for use on edge devices (e.g. ONNX, TensorFlow Lite)


Timeline
___
Competition starts on 4 October 2024 at 8:00 AM GMT.

Competition closes on 15 December 2024.

Final submissions must be received by 11:59 PM GMT.

We reserve the right to update the contest timeline if necessary.
