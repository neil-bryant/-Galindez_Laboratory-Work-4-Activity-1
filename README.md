# -Galindez_Laboratory-Work-4-Activity-1

Google Drive link:  
https://drive.google.com/drive/folders/1fz8Q_8FbA6DLB_MX6TLE2_w4T-x489TN?usp=sharing

Google Collab: 
https://colab.research.google.com/drive/1SWklnl74NRovMGJHQUYWId22sXToPr2_?usp=sharing

Activity 3: Model Enhancement and Performance Optimization
Guide Questions — Student Explanation & Reflection

What were the weakest-performing classes based on the confusion matrix? 
The weakest-performing class was Epidendrum, which was most frequently misclassified as Masdevallia 36 times, indicating significant visual similarity between the two orchid species. In comparison, Marriot showed only minor misclassification, being confused with Cymbidium just 3 times, making Epidendrum the most challenging class for the model to distinguish correctly.

How did Precision, Recall, and F1-score vary across classes?
Most classes achieved perfect or near-perfect Precision, Recall, and F1-scores (1.00). However, Epindendrum had the lowest Recall (0.40) and F1-score (0.57), meaning the model missed many actual instances despite having perfect Precision (1.00). Masdevallia had the lowest Precision (0.61) but perfect Recall (1.00), showing frequent incorrect predictions. Marriot showed slightly lower performance with a Recall of 0.95 and F1-score of 0.97 due to minor misclassifications.

What does a low recall indicate in your model?
A low recall indicates that the model fails to correctly identify many actual instances of a class. For example, Epindendrum had a recall of 0.40, meaning only 40% of its actual images were correctly classified, while the remaining 60% were misclassified into other classes.


How does AUC score reflect model performance compared to accuracy?
Accuracy measures the overall percentage of correct predictions, while AUC measures how well the model can distinguish between classes across different thresholds. A higher AUC indicates better class separation and is often more reliable than accuracy, especially for imbalanced datasets, because it is less affected by class distribution.



B. Model Improvement
How did data augmentation affect validation accuracy?
Data augmentation significantly improved validation accuracy from 96.00% in the baseline model to 100.00% in the enhanced model. By applying flips, rotations, zooms, and brightness/contrast adjustments, the model was exposed to more varied training images, which improved generalization and reduced overfitting.

Why is Batch Normalization important in CNNs?
Batch Normalization is important in CNNs because it stabilizes learning by normalizing layer inputs, speeds up training through faster convergence, improves gradient flow to prevent vanishing or exploding gradients, and helps reduce overfitting by adding a slight regularization effect.

What role did Dropout play in improving your model? 
Dropout helped improve the model by preventing overfitting. It randomly disables some neurons during training, forcing the network to learn more robust and generalized features instead of relying on specific neurons. This improved the model’s performance on unseen validation data.

How did Early Stopping prevent overfitting?
Early Stopping prevented overfitting by monitoring validation performance during training and stopping the process once the validation loss stopped improving for several epochs. It also restored the best model weights, ensuring the model did not continue training after it began overfitting the training data.

C. Performance Comparison
What improvements were observed after modifying the model?
After modifying the model, all performance metrics improved significantly. Validation accuracy increased from 96.00% to 100.00%, while Macro Precision, Recall, and F1-score also reached 100.00%. The AUC score improved from 95.97% to 99.96%, showing better overall classification and class separation performance.

Which enhancement contributed the most to performance improvement? Why? 
It's difficult to pinpoint a single
