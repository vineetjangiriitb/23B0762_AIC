Architecture:

Transformer Architecture: Vision-Based Transformers are adapted from the transformer architecture originally designed for natural language processing (NLP).
They rely heavily on self-attention mechanisms to process and understand the input data.
Patch Embedding: Instead of processing entire images as a whole, ViTs divide images into fixed-size patches (e.g., 16x16 pixels). Each patch is then linearly
embedded into a vector, creating a sequence of patch embeddings similar to word embeddings in NLP.

Self-Attention Mechanism:

Global Context: Self-attention allows ViTs to consider relationships between all patches in the image simultaneously, capturing global context more effectively
than CNNs, which typically have a more localized receptive field.
Positional Encoding: Since the transformer architecture does not inherently capture spatial information, positional encodings are added to patch embeddings to
retain spatial relationships within the image.

Comparison with CNN-Based Models:

Training Data Requirements:
CNNs: Perform well with relatively smaller datasets due to the inductive biases introduced by convolutions and pooling layers, which help them generalize from 
fewer examples.
ViTs: Often require significantly larger datasets to achieve comparable performance because they lack these inductive biases. However, pre-training on large datasets
(e.g., ImageNet) and fine-tuning on specific tasks can mitigate this requirement.

Efficiency and Complexity:
CNNs: Generally more efficient in terms of computational resources for smaller images due to localized convolutions and pooling operations. They also benefit from
extensive optimization in hardware and software over the years.
ViTs: Can be more computationally intensive, especially for large images, due to the quadratic complexity of the self-attention mechanism (with respect to the number
of patches). However, ViTs have shown that with sufficient data and computational power, they can achieve superior performance.

Feature Extraction:
CNNs: Utilize convolutional layers to extract hierarchical features, starting with low-level features (e.g., edges, textures) and progressing to high-level features
(e.g., object parts, entire objects).
ViTs: Rely on self-attention to capture feature representations from the entire image. Each layer in a ViT aggregates information globally, which can lead to a more
holistic understanding of the image content.

Performance and Accuracy:
CNNs: Have been the state-of-the-art in many computer vision tasks and are well-understood in terms of architecture design, training, and optimization.
ViTs: Recent research has shown that ViTs can outperform CNNs on several benchmarks, particularly when trained on large datasets. They have demonstrated strong
performance in tasks such as image classification, object detection, and segmentation.

Sources of information:
https://arxiv.org/pdf/2010.11929
https://chatgpt.com/c/3def7d13-bdd3-4c55-9449-99bfa53fd82e



