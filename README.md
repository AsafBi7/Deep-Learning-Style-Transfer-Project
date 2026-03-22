# Bring Van Gogh Back to Life: Style Transfer & Classification
This project explores the intersection of computer vision and art history by training a deep learning "Art Expert" to recognize Vincent van Gogh's style and subsequently using generative techniques to recreate it.

It was completed as part of the "Introduction to Deep Learning" course during my B.Sc. in Data Science at Tel Aviv University. The project demonstrates the practical application of Convolutional Neural Networks (CNNs) for both discriminative (classification) and generative (style transfer) tasks.

The analysis includes training architectural comparisons between VGG-19 and AlexNet, implementing Neural Style Transfer (NST), and performing a cross-model evaluation where the trained classifier acts as a critic for the generated artwork.

### Project Objectives
* Train a robust classifier to distinguish authentic Van Gogh works from other Post-Impressionist paintings.

* Implement Neural Style Transfer to apply Van Gogh’s iconic brushwork to arbitrary content images.

* Compare the performance of VGG-19 and AlexNet in capturing semantic structure vs. artistic texture.

* Evaluate generative results using a "Strict Critic" (the trained classifier) to measure stylistic success.

### Files Included
* `Final_ProjectQ1_New.ipynb` - Data preprocessing, architecture definition, and training of the "Art Expert" classifiers.

* `Final_ProjectQ2.ipynb` - Implementation of the Style Transfer algorithm and the automated evaluation pipeline.

* `Part 3_ Discussion & Analysis.pdf` - Detailed technical report analyzing model depth, hierarchical features, and the "circular validation trap."

* `Deep learning project 2026.pdf` - Original project specifications and academic requirements.

### Deep Learning Models Used
* **VGG-19**: Utilized for its deep hierarchical feature extraction, proving superior in preserving image structure.

* **AlexNet**: Used as a baseline to demonstrate the trade-offs between computational efficiency and stylistic depth.

### Key Techniques
* **Transfer Learning:** Leveraging pre-trained ImageNet weights for specialized art classification.

* **Neural Style Transfer (NST):** Optimization-based generation using Gram matrices for style representation.

* **Architectural Analysis:** Investigation into why deeper networks (VGG) separate content from style more effectively than shallower ones (AlexNet).

* **GPU Acceleration:** High-performance training and inference utilizing NVIDIA RTX 4090.
