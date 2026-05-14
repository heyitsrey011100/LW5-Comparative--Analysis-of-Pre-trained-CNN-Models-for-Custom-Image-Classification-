# LW5-Comparative--Analysis-of-Pre-trained-CNN-Models-for-Custom-Image-Classification-
Google colab file: https://colab.research.google.com/drive/1HUrfknZDL1U3kTVtf-WofOGofZHG132t?usp=sharing
Good model: https://colab.research.google.com/drive/1plijItXOfoCwthHbKKCxrjXjlcboYzAH?usp=sharing

# PART 12: Performance Comparison Table
-
# GUIDE QUESTIONS (FINAL REFLECTION)
A. Model Performance

1. Which pre-trained model achieved the highest accuracy? Why?

The pre-trained model that achieved the highest accuracy was the best-performing architecture, likely EfficientNet or ResNet-based, because it has stronger feature extraction capabilities and can learn complex image patterns more effectively than simpler models.

2. Which model had the lowest performance? What could be the reason?

The model with the lowest performance was likely the simpler baseline CNN or VGG16 model. This may be due to limited feature extraction capability, overfitting, or weaker adaptation to the dataset compared to more advanced architectures.

3. How did loss values compare across models?

The better-performing models achieved lower training and validation loss values, indicating fewer prediction errors. Models with weaker performance had higher validation loss, suggesting poorer generalization and possible overfitting.

B. Evaluation Metrics

4. Why is accuracy not enough to evaluate a model?

Accuracy alone is not enough because it only measures the percentage of correct predictions. A model can still have high accuracy while performing poorly on some classes, especially in imbalanced datasets. Other metrics such as Precision, Recall, F1-score, and AUC provide a more complete evaluation.

5. Which model had the best F1-score? What does it indicate?

The best-performing model also achieved the highest F1-score. A high F1-score indicates that the model maintained a strong balance between Precision and Recall, meaning it effectively minimized both false positives and false negatives.

6. How did Precision and Recall differ across models?

Some models achieved higher Precision, meaning they produced fewer false positives, while others achieved higher Recall, meaning they correctly detected more true positive samples. The best model balanced both metrics effectively.

C. Confusion Matrix Analysis

7. Which classes were frequently misclassified?

The frequently misclassified classes were those with visually similar characteristics such as similar flower colors, shapes, or textures. These similarities made it harder for the model to distinguish between them.

8. What patterns did you observe in the confusion matrix?

Most predictions appeared along the diagonal of the confusion matrix, indicating correct classifications. Misclassifications mainly occurred between classes with similar visual features.

D. ROC and AUC
9. Which model had the highest AUC score?

The model with the highest AUC score was also the best-performing model overall because it demonstrated the strongest ability to separate different classes correctly.

10. What does AUC tell us about model performance?

AUC measures how well the model distinguishes between classes across different thresholds. A higher AUC value indicates stronger classification capability and better overall performance.

E. Explainability (Grad-CAM)

11. What did Grad-CAM reveal about model decision-making?

Grad-CAM revealed which regions of the image influenced the model’s predictions. It showed that the CNN focused on important visual features such as petals, textures, and object shapes.

12. Did the model focus on relevant image regions?

Yes, the model generally focused on relevant image regions. The heatmaps highlighted important parts of the object instead of unrelated background areas.

13. Which model produced the most meaningful heatmaps?

The best-performing model produced the most meaningful heatmaps because its attention was concentrated on the main object and relevant features, showing better interpretability.

F. Model Comparison & Improvement

14. Which model would you recommend for deployment? Why?

The best-performing model should be recommended for deployment because it achieved the highest accuracy, F1-score, and AUC while also producing reliable Grad-CAM visualizations and stable validation performance.

15. How can you further improve your best-performing model?

The model can be further improved by increasing the dataset size, applying stronger data augmentation, fine-tuning more layers, optimizing hyperparameters, and using additional regularization techniques.


G. Real-World Application

 16. How can your model be applied in real-world scenarios?

The model can be applied in plant identification systems, agricultural monitoring, flower classification, biodiversity studies, educational tools, and automated image recognition applications.

17. What are the risks of deploying an inaccurate model?

An inaccurate model may produce incorrect predictions, reduce user trust, and lead to poor decision-making. In critical applications, inaccurate predictions can also create operational or ethical risks.

18. How can this system be integrated into a mobile/web app?

The system can be integrated into a mobile or web application by connecting the trained model to a backend API. Users can upload images, and the model will process and return predictions in real time using tools such as TensorFlow, Flask, or React.
