🩺 ODIR5K Retinal Disease Classification using Deep Learning


<p align="left"> <img src="https://img.shields.io/badge/Python-3.10-blue.svg"> <img src="https://img.shields.io/badge/TensorFlow-2.x-orange.svg"> <img src="https://img.shields.io/badge/Keras-DeepLearning-red.svg"> <img src="https://img.shields.io/badge/Medical-AI-green.svg"> </p>
<img width="1134" height="496" alt="WhatsApp Image 2026-06-29 at 7 49 54 PM" src="https://github.com/user-attachments/assets/0c721dae-ad9e-42b4-a5ea-80294e4968ab" />

ODIR5K Retinal Disease Classification:



This project presents a deep learning framework for automated retinal disease classification using fundus images from the ODIR-5K dataset. Early diagnosis of retinal diseases is critical because untreated ocular disorders can lead to irreversible vision impairment and blindness. Traditional diagnosis requires highly trained ophthalmologists and considerable clinical effort. Therefore, computer-aided diagnosis systems based on artificial intelligence can provide rapid, accurate, and scalable screening solutions.
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/71af7cf4-5e3d-46d2-aa24-d2921658f805" />
The proposed model leverages convolutional neural networks for hierarchical feature extraction from retinal fundus images. Extensive preprocessing, augmentation, transfer learning, and performance evaluation techniques were employed to develop a robust classification pipeline capable of identifying multiple retinal diseases from fundus photographs.

Dataset:

The project utilizes the ODIR-5K (Ocular Disease Intelligent Recognition) dataset containing retinal fundus images collected from real clinical environments.

The dataset includes multiple retinal disease categories:

Normal Retina
Diabetic Retinopathy
Cataract
Glaucoma
Pathological Myopia
Hypertension
Age-related Macular Degeneration
The ODIR dataset is widely used in ophthalmic artificial intelligence research because it contains diverse retinal abnormalities captured under real-world clinical conditions. The significant class imbalance and image variability make retinal disease classification a challenging computer vision problem. Recent research has shown that combining CNN-based local feature extraction with transformer-based global feature modeling can significantly improve retinal disease diagnosis performance.

Confusion Matrix Analysis

The confusion matrix is a visual representation of the classification performance of the proposed retinal disease classification model. The rows represent the actual (true) disease classes, while the columns represent the predicted disease classes. The diagonal values correspond to correctly classified samples, whereas the off-diagonal values indicate misclassifications.
<img width="932" height="790" alt="image" src="https://github.com/user-attachments/assets/96dcf640-4fe4-4c7d-afc6-67638557938b" />


Overall Performance

The proposed model achieved an overall classification accuracy of approximately 84.10%, demonstrating strong performance across seven retinal disease categories. Most predictions are concentrated along the diagonal of the confusion matrix, indicating that the model successfully learned discriminative features for retinal disease identification.

Clinical Interpretation

The confusion matrix demonstrates that the proposed deep learning model can effectively distinguish major retinal diseases while maintaining high diagnostic sensitivity. However, diseases with subtle retinal abnormalities, such as diabetic retinopathy and early-stage glaucoma, remain challenging due to their visual similarity to healthy retinal structures. Future improvements may include attention mechanisms, Vision Transformers, ensemble learning, and explainable AI techniques such as Grad-CAM to enhance diagnostic reliability.

Retinal Disease Image Analysis

The figure above presents representative retinal fundus images belonging to two clinically significant ocular disorders: Diabetic Retinopathy (left) and Glaucoma (right). Retinal fundus imaging is a non-invasive diagnostic technique that provides detailed visualization of the retina, optic disc, blood vessels, and macula, allowing ophthalmologists to identify pathological changes associated with various retinal diseases.

Diabetic Retinopathy
<img width="1600" height="500" alt="image" src="https://github.com/user-attachments/assets/54294a41-6f76-46b4-8c13-c22a2080810e" />

The image on the left illustrates a retinal fundus affected by Diabetic Retinopathy (DR), one of the leading causes of vision impairment worldwide. Diabetic retinopathy occurs due to prolonged hyperglycemia, which damages the retinal microvasculature and causes leakage, hemorrhage, and ischemia. Several characteristic pathological features can be observed in the image, including:

Microaneurysms
Retinal hemorrhages
Hard exudates
Cotton wool spots
Vascular abnormalities

These lesions appear as bright yellow-white deposits and scattered hemorrhagic regions across the retina. The presence of multiple exudates and vascular changes indicates retinal damage caused by diabetes mellitus. Early detection of diabetic retinopathy is critical because timely treatment can significantly reduce the risk of permanent vision loss.

Training and Validation Performance Analysis

The performance of the proposed retinal disease classification model was evaluated over 20 training epochs using training and validation accuracy and loss metrics. These learning curves provide valuable insights into the convergence behavior, generalization capability, and overall effectiveness of the deep learning model.

Model Accuracy Analysis

The accuracy curve demonstrates the evolution of classification performance throughout the training process. The training accuracy increased steadily from approximately 72.5% during the initial epoch to 80.8% by the final epoch, indicating that the model successfully learned discriminative retinal features from the training dataset.
<img width="1390" height="490" alt="image" src="https://github.com/user-attachments/assets/49c52186-bf47-4dd1-8283-34fe3db99f3a" />


Similarly, the validation accuracy rapidly improved during the early training stages and stabilized around 83–84%, achieving a peak validation accuracy of approximately 84.1%. The relatively small difference between training and validation accuracy suggests that the model exhibits strong generalization performance and does not suffer from significant overfitting.

The validation accuracy consistently remained higher than the training accuracy throughout the training process. This behavior is commonly observed when regularization techniques such as data augmentation, dropout, batch normalization, and transfer learning are employed, as these methods improve the model's ability to generalize to unseen retinal images.

Key observations from the accuracy curve include:
Steady increase in training accuracy throughout training.
Rapid convergence of validation accuracy.
Stable performance after approximately 10 epochs.
Minimal gap between training and validation accuracy.
Absence of severe overfitting.

Model Loss Analysis

The loss curves illustrate the optimization behavior of the neural network during training. The training loss decreased significantly from approximately 0.95 during the first epoch to around 0.57 at the final epoch, demonstrating effective parameter optimization and feature learning.

Similarly, the validation loss decreased from approximately 0.59 to 0.48, indicating that the model maintained strong predictive performance on previously unseen retinal images. The smooth decline in both training and validation loss confirms the stability of the optimization process and the effectiveness of the chosen learning strategy.

The validation loss remained consistently lower than the training loss throughout the training process, further supporting the conclusion that the model generalizes well and benefits from regularization techniques.
