# Garbage Classifier Using Image and Text Data

This project implements a garbage classification model that leverages both image and textual description inputs. The classifier is designed to predict the type of garbage based on an image of the item and a short descriptive text.

## Approach

1. **Image Model**: The image classifier uses VGG19, trained through transfer learning, achieving an accuracy of approximately **63%**.
2. **Text Model**: The text classifier is based on XLM-RoBERTa, also trained through transfer learning, with an accuracy of around **84%**.

## Model Fusion

To improve the classifier's performance, we experimented with different fusion weights for combining the predictions from the image and text models. Specifically, we tested weight combinations of **0.25:0.75**, **0.5:0.5**, and **0.75:0.25** for the image and text models, respectively. The fused model achieves an average accuracy of **78%** across these configurations.

