# 🧠 Building simplified models of primary visual cortex (V1) 🐭 🐵

**Student notebook -->** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](...)

**Instructor notebook -->** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](...) 

**By Fengtong(Farah) Du and Carsen Stringer**

In this tutorial, we will build predictive models of V1 neural activity from visual stimuli (natural images). The predictive models are:

1.   linear regression
2.   one convolutional layer (shared across neurons) + neuron-specific readout
3.   2-convolutional layer net + neuron-specific readout with separable convolutions
4.   small neuron-specific "minimodels" with 2 convolutional layers + readout.

For each of these models, we will visualize the weights to help us understand the feature selectivity of V1 neurons.

This notebook uses [code](https://github.com/mouseland/minimodel) and [data](https://janelia.figshare.com/articles/dataset/Towards_a_simplified_model_of_primary_visual_cortex/28797638) from [Du et al 2025](https://www.nature.com/articles/s41467-025-61171-9). If you use any code or data from this notebook, please cite the paper.
