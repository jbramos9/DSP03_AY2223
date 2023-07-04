# Multi-Stage Hybrid-CNN Transformer Model for Human Intent-Prediction
This repo contains all the models (including the variant) developed in the project [ Multi-Stage Hybrid-CNN Transformer Model for Human Intent-Prediction](). As an overview, the Multi-Stage Hybrid-CNN Transformer Classifier System is composed of two key components: the Gazed Object Detector and the Intent Classifier.
- The Gazed Object Detector is in the `gazed_object_detectors` which contains the three different variations of the model.
- The Intent Classifier is in the `intent_classifier` folder.
- Additionally, the overall system for inference is in the `multi-stage_human_intent_classifier_system` folder. To learn more about each model, each folder contains its own readme.md for guidance.

### Recommendations
1. Add more video samples such that the gaze distribution is balanced ("None" or not looking at objects is currently overrepresented)
2. Develop the weights of the Gaze Object Detector from scratch to tailor the model for object-gaze classification
3. Consider the probability of gaze for all objects in a given frame, instead of the most probable gaze, as input to the human intent classifier
4. Explore other human pose estimation techniques (as inspired by the increase in performance from the additional head information used)
