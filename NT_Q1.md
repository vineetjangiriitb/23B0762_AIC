Q.1] Problem statement for competition
Image Matching Challenge 2024 - Hexathlon (Reconstruct 3D scenes
from 2D images over six different domains)
The goal of this competition is to construct precise 3D maps using sets
of images in diverse scenarios and environments. You’ll develop a
model to generate accurate spatial representations, regardless of the
source domain—images taken from drones, amidst dense forests,
during nighttime, or any of the six problem categories.

Preparation Timeline(1-Month) for AI Based Hackathon

Week 1: Understanding and Planning:
Day 1-2: Define Goals and Assemble the Team
• Goal Setting: Understanding the project goals, deliverables,
competition rules and evaluation metrics.
• Team Formation: Assemble a diverse team of core enthusiast and
having great knowledge and experience of such AI projects.
Day 3-4: Problem Understanding and Literature Review
• Problem Breakdown: Analyzing the problem statement,
understanding and focusing on the requirements for constructing
3D maps from 2D images across six domains.
• Literature Review: Research of existing methods in image
matching, 3D reconstruction from 2D images, and domain
adaptation. Review state-of-the-art techniques and relevant
academic papers. Finding similar kind of works in AI communities
and forums to gain more insights.
Day 5-7: Data Examination and Compute Setup
• Dataset Familiarization: Reviewing the provided datasets to
understand their structure and contents. Identify the six different
domains and examine a sample from each to get a sense of the
variety and challenges in the dataset. Conduct EDA(Exploratory
Data Analysis) to understand the characteristics of the datasets.
Use tools like Matplotlib and Seaborn for visualizations.
• Compute Setup: Setting up cloud resources or local high-
performance computing infrastructure. Ensuring access to GPUs,
storage, and necessary software.

Week 2: Data Preprocessing and Model Development:
Day 8-10: Data Preprocessing
• Data Cleaning: Handle any remaining missing values, outliers, and
inconsistencies in the training dataset.
• Normalization and Augmentation: Apply normalization techniques
and data augmentation to improve model robustness. Techniques
may include rotations, scaling, and color jittering.
• Label Preparation: Ensure that all datasets are properly labeled
and segmented and object positions are clearly identified and
marked.
• Finding overlaps: Finding overlapping regions and mapping
between different images is important for constructing 3D spatial
models.
Day 11-14: Model Selection and Prototyping
• Model Research: Research and select suitable models for image
matching and 3D reconstruction, such as CNNs for feature
extraction, and depth estimation models.
• Prototyping: Implement initial versions of selected models using
frameworks like TensorFlow or PyTorch.
• Testing and selection: Testing the prototype models on various
criterias and selecting best framework for training purposes.

Week 3: Model Training and Evaluation:
Day 15-18: Training and Hyperparameter Tuning
• Model Training: Train models on each domain-specific dataset.
Monitor training progress using metrics like (both validation and
training) loss and accuracy. Early stopping(optional) is beneficial
many times when required accuracy levels are reached and further
training might not be much beneficial.
• Hyperparameter Tuning: Perform hyperparameter tuning using
techniques like grid search or Bayesian optimization.
Day 19-22: Model Evaluation
• Cross-Domain Testing: Evaluate models across different domains
to ensure generalization. Use metrics such as F1 score, confusion
matrix, Mean Squared Error (MSE), Intersection over Union (IoU),
and 3D reconstruction accuracy.
• Validation and Testing: Split data into training, validation, and
testing sets. Conduct thorough testing to evaluate performance.
• Re-training experimentations: Models can be trained by making
some variations and using various measures like layer dropout,
regularization to ensure better fitting of model.

Week 4: Model Optimization and Finalization
Day 23-25: Model Optimization
• Optimization Techniques: Apply techniques like model pruning,
quantization, and efficient architectures (e.g., MobileNets) to
optimize for speed and memory usage.
• Ensemble Methods: Using ensemble methods to combine multiple
models for improved accuracy.
Day 26-28: Final Preparations and Submission
• Model Integration: Integrate different components and ensure the
final model pipeline is robust and efficient.
• Documentation: Prepare detailed documentation, including model
descriptions, methodologies, and instructions for running the code.
• Submission Preparation: Package the model and documentation
according to competition requirements. Conduct a final review to
ensure all criteria are met.
Day 29-30: Some buffer time for any final moment modifications
and to cover any delays in any processes
