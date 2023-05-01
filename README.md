# Data-Challenge-Face-Recognition

### Data Challenge proposed by IDEMIA in the Advanced Master in Artificial Intelligence at Télécom Paris (2021-2022).

This is my work for the Data Challenge proposed by IDEMIA dealing with fairness in face recognition system.

### Author : Davide Garcia Civiero

### Presentation of the challenge : face recognition

#### How does modern face recognition work?
In the past few years, Face Recognition (FR) systems have reached extremely high levels of performance, paving the way to a broader range of applications, where the reliability levels were previously prohibitive to consider automation. This is mainly due to the adoption of deep learning techniques in computer vision. The most adopted paradigm consists in training a network $f: \mathcal{X} \rightarrow \mathbb{R}^d$ which, from a given image $im \in \mathcal{X}$, extracts a feature vector $z \in \mathbb{R}^d$ which synthetizes the relevant caracteristics of $im$. The recognition phase then consists, from two images $im_1, im_2$, to predict wether they correspond to the same identity or not. This is done from the extracted features $z_1, z_2$. 
#### What you are ask to do
In this data challenge, you are ask to train a machine learning model which, from a vector $[z_1, z_2]$ made of the concatenation of two templates $z_1$ and $z_2$, predict wether or not these two images correspond to the same identity.  

### Peformance criterion

You are asked to minimize the sum of the False Positive Rate (FPR) and the False Negative Rate (FNR).
Your score is calculated using below equation.

score = 1 - (FPR + FNR)
