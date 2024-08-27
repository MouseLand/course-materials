# course-content

## Installing locally:

If you are using a GPU, make sure its drivers and the cuda libraries are correctly installed.

1. Install a [miniforge](https://github.com/conda-forge/miniforge) distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
2. Open an anaconda prompt / command prompt which has `conda` for **python 3** in the path
3. Create a new environment with `conda create --name mouseland python=3.10`.
4. To activate this new environment, run `conda activate mouseland`
5. Install jupyter notebook with `python -m pip install notebook`.
6. In this terminal, run `jupyter-notebook` to open a jupyter notebook in your browser.

Now you can download the notebooks and open them there.

If you'd like to try out the GUI version of cellpose or rastermap, you can install them with the following commands:
~~~sh
python -m pip install cellpose[gui]
python -m pip install rastermap[gui]
~~~

Use "" around "cellpose[gui]" if on zsh. Note you will always have to run `conda activate mouseland` before you run cellpose or rastermap.

### [Cellpose segmentation and signal extraction for calcium imaging data](cellpose_extraction/)

Student notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/course-materials/blob/main/cellpose_extraction/tutorial.ipynb)

Instructor notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/course-materials/blob/main/cellpose_extraction/tutorial_solutions.ipynb)

This notebook will guide you through the stages of processing two-photon data. This is data collected from a wild-type mouse injected with GCaMP6s in layer 2/3 of primary visual cortex. The mouse was head-fixed above a ball and free to run, with no visual input (lights turned off). The recording was collected at 13Hz (there were 3 planes in the recording, 1 is included here). The recording has already been registered - in practice, you will need to run motion registration first. We will cover the subsequent steps of imaging data:

1. cell detection with [cellpose](https://github.com/mouseland/cellpose)
2. signal extraction
3. visualization with [rastermap](https://github.com/mouseland/rastermap)

### [Behavioral encoding models of neural population activity](behavior_encoding/)

Student notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/course-materials/blob/main/behavior_encoding/tutorial.ipynb)

Instructor notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/course-materials/blob/main/behavior_encoding/tutorial_solutions.ipynb)

We will use a spontaneous activity recording from [Syeda et al, 2023](https://www.biorxiv.org/content/10.1101/2022.11.03.515121v1.abstract). We recorded 34,086 neurons from mouse sensorimotor cortex for 2+ hours using two-photon calcium imaging at a rate of 3.2Hz. In the notebook, we will build several encoding models of neural activity based on the orofacial behaviors of mice. The encoding models are increasingly more complicated:

1. linear regression from spatial keypoints
2. linear regression from spatiotemporal keypoints
3. nonlinear regression (i.e. neural networks) from spatiotemporal keypoints

We will use [rastermap](https://github.com/mouseland/rastermap) to visualize the neural activity, and also to visualize the prediction.


