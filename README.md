# SSL Cookbook

[A Cookbook of Self-Supervised Learning](https://arxiv.org/abs/2304.12210)

This page is for 1. documenting the structure of the cookbook; 2. TLDR - taxonomies of SSL; 3. scribing pieces with nice wordings (?).

# Intro

- SSL defines a pretext task based on unlabeled inputs to produce descriptive and intelligible representations.
- NLP and CV examples
- While traditional supervised learning methods are trained on a specific task often known as a priori based on the available labeled data, SSL learns generic representations useful across many tasks.
- SECTION2: SSL techniques
- SECTION3: Practical considerations to implement SSL

# Families and origins of SSL

- Origins of SSL
    
    (foundation of modern methods, may longer be state-of-the-art)
    
    - Information restoration
        - colorization (requires understanding of obj semantics); masked image recovery (MAE)
    - Using temporal relationships in video
        - videos contain multiple modalities of info that can be masked
    - Learning spatial context
        - predicting object orientations; relative locations of random image patches; counting objects
    - Grouping similar images (clustering)
        - Creating informative feature-space clusters
    - Generative models
        - restoration-based autoencoders; GANs
    - Multi-view invariance
        - contrastive learning;
    
    **Four SSL families:**
    
    1. Deep Metric Learning
    2. Self-Distillation
    3. Canonical Correlation Analysis
    4. Masked Image Modeling
- Deep Metric Learning (SimCLR/NNCLR/MeanSHIFT/SCL)
    
    The deep metric learning family is based on the principle of encouraging similarity between semantically transformed versions of an input.