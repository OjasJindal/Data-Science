In this experiment, different sampling techniques were applied to a highly imbalanced credit card fraud dataset to study their effect on the performance of multiple machine learning models. Initially, the dataset was dominated by non-fraud transactions, which is a common real-world problem in fraud detection systems. Such imbalance can mislead machine learning models into favoring the majority class and ignoring important minority cases.

After balancing the dataset and applying five sampling methods — Simple Random Sampling, Stratified Sampling, Bootstrap Sampling, Oversampling, and Undersampling — noticeable differences in model performance were observed. This clearly shows that the choice of sampling technique plays an important role in improving classification accuracy.

Simple Random Sampling provided stable and consistent results for most models, but it did not always preserve the class distribution effectively. Stratified Sampling performed better in maintaining proportional class representation, which helped some models learn more balanced decision boundaries. This was especially useful for algorithms that are sensitive to data distribution.

Bootstrap Sampling helped improve model robustness by training on randomly resampled data with replacement. This technique was useful in reducing variance for certain models, particularly ensemble-based models like Random Forest. However, because duplicate samples are introduced, it may sometimes lead to slight overfitting.

Oversampling showed strong performance for models such as Random Forest and Support Vector Machine. By increasing the number of minority class samples, the models were able to better learn fraud patterns. This technique is especially helpful when the minority class contains important but limited information. However, oversampling can increase training time and may also introduce redundancy.

Undersampling reduced the size of the majority class to create balance. While this improved training speed, it also caused a loss of valuable information from the dataset. As a result, some models showed lower accuracy when undersampling was applied, especially those that rely on large datasets for better learning.

Overall, the experiment demonstrates that no single sampling method is best for all machine learning models. Each model reacts differently depending on how the data is prepared. Therefore, selecting the right sampling strategy should depend on the dataset characteristics and the type of algorithm being used.

This study highlights the importance of proper data preprocessing in real-world applications such as fraud detection. Effective sampling techniques not only improve model performance but also make predictions more reliable and practical for deployment
