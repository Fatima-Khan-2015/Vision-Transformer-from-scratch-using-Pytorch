# Vision-Transformer-from-scratch-using-Pytorch

Dataset

The project uses the Oxford-IIIT Pet Dataset, which consists of 37 categories of pet images (different breeds of cats and dogs). Each image is labeled with its class, making this a multiclass classification problem. The dataset includes significant variation in scale, pose, and lighting, which makes it a good benchmark for testing image classification models.

Model

A Vision Transformer (ViT) was implemented from scratch using PyTorch and the einops package. The model was trained using:

Optimizer: AdamW

Learning Rate: 0.001

Loss Function: CrossEntropyLoss

Epochs: 50

Batch Size: 32

Final Results

At the end of training, the model was evaluated on a test batch. The outputs were:

Predicted classes: A list of class indices assigned by the Vision Transformer.

Actual classes: The ground-truth labels from the dataset.

The results showed that the model could correctly predict several of the pet categories, although some misclassifications were present. This indicates that the ViT successfully learned distinguishing features of the dataset, but with room for improvement in generalization.

Conclusion

The Vision Transformer trained on the Oxford-IIIT Pet dataset demonstrated the ability to classify pet breeds into their respective categories. With 50 epochs of training at a learning rate of 0.001, the model reached a point where its predictions aligned with many of the actual classes, though further fine-tuning (longer training, data augmentation, learning rate scheduling) could improve accuracy.
