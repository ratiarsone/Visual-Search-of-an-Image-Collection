This repository presents the design, implementation, and evaluation of a visual image retrieval
system tested on the MSRC-v2 dataset (591 images, 20 object categories). Starting from a
global colour histogram baseline (mAP = 0.167), I systematically investigated how spatial
encoding, dimensionality reduction, alternative descriptors, feature fusion, and deep learning
affect retrieval performance. Spatial grid colour histograms provided marginal improvement
in raw form but benefited substantially from PCA compression (mAP = 0.188 at 32
components). Combining colour and edge orientation descriptors achieved mAP = 0.240, and
fusing all handcrafted features with Bag of Visual Words reached 0.253. A pretrained
ResNet18 CNN descriptor achieved 0.725 with cosine distance, demonstrating the dominance
of learned representations over handcrafted features. Throughout the investigation, I found
that descriptor dimensionality, distance metric choice, and feature complementarity were
more important than any single descriptor design decision.
