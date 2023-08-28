# course-content

### [Behavioral encoding models of neural population activity](behavior_encoding/)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb)

We will use a spontaneous activity recording from [Syeda et al, 2023](https://www.biorxiv.org/content/10.1101/2022.11.03.515121v1.abstract). We recorded 34,086 neurons from mouse sensorimotor cortex for 2+ hours using two-photon calcium imaging at a rate of 3.2Hz. In the notebook, we will build several encoding models of neural activity based on the orofacial behaviors of mice. The encoding models are increasingly more complicated:

1. linear regression from spatial keypoints
2. linear regression from spatiotemporal keypoints
3. nonlinear regression (i.e. neural networks) from spatiotemporal keypoints

We will use [rastermap](https://github.com/mouseland/rastermap) to visualize the neural activity, and also to visualize the prediction.


