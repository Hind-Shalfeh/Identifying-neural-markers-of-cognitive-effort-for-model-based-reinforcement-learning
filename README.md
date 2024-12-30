# Identifying-neural-markers-of-cognitive-effort-for-model-based-reinforcement-learning
# 

### Abstract

This study investigates the biological plausibility of cognitive effort in artificial neural networks (ANNs) through a comparative analysis of human and ANN behavior in decision-making tasks. Using tasks adapted from Kool et al. (2017), two types of decision-making strategies—model-based and model-free—are evaluated. The ANNs are trained using the REINFORCE algorithm on custom environments designed to mimic experimental paradigms applied to human participants which are the two-step task and a novel version of the two-step task (kool at al. 2017).
---

## **Repository Overview**

This repository contains a code, which investigates cognitive effort in artificial neural networks (ANNs). The main components of this repository are as follows:

- **Custom Gymnasium Environments**: These environments are designed to mimic the decision-making tasks used in human participant experiments the first is the original Two-step Task, the second is a novel variant of the two-step task.
- **Reinforcement Learning**: ANNs are trained using the **REINFORCE algorithm** (code based on code from Christian cancedda)on these environments.
- **Data Analysis**: The repository also includes code for analyzing the network's activities plotting stay probabilities and comparing performance between human and artificial neural networks.

The repository consists of **6 Jupyter notebooks**, each performing different tasks. All notebooks can be run independently, and the required imports and installations are already included within each notebook.

---

## **Repository Structure**

There are no specific folders, but the following files are included in the repository:

1. **Training Notebooks:**
   - `Training_NN_on_Original_Task.ipynb`: Trains a neural network on the original two-step decision-making task.
   - `Training_NN_on_Novel_Task.ipynb`: Trains a neural network on the novel two-step decision-making task.

2. **Testing Notebooks:**
   - `Testing_Trained_vs_Untrained_NN_Original_Task.ipynb`: Tests the trained network on the original two-step task environment (trained vs. untrained) and contains the code for plotting stay probabilities and average accumalative rewards.
   - `Testing_Trained_vs_Untrained_NN_Novel_Task.ipynb`: Tests the trained network on the novel two-step task environment (trained vs. untrained) and contains the code for plotting stay probabilities and average accumalative rewards.

3. **Network Activity Notebook:**
   - `Summing_up_Activities_NN_on_Original_Task.ipynb`: Summarizes the activities of the network units as it interacts with the environment and plots them.

4. **Data Comparison Notebook:**
   - `Comparing_human_vs_NN_Preformance.ipynb`: Compares and visualizes the dataframes collected during testing with human choices on the same tasks from (koo et al. 2017). The dataframes generated with this project are available via a [Google Drive link](https://drive.google.com/drive/folders/1iWpeb9lCzxbTarJf0iIszwamrjgRb9FV?usp=drive_link).

---

## **Installation Requirements**

The code is implemented in **Python** and uses the following libraries:

- **PyTorch** (for building and training the neural networks)
- **NumPy** (for numerical operations)
- **Matplotlib** (for visualizations)
- **Pandas** (for data handling)
- **gymnasium** (for running the environments)

To install the required libraries, use the `requirements.txt` file provided in the repository. Simply run:

```bash
pip install -r requirements.txt


references:
Kool, W., Gershman, S. J., & Cushman, F. A. (2017). Cost-Benefit Arbitration Between Multiple Reinforcement-Learning Systems. Psychological science, 28(9), 1321–1333. https://doi.org/10.1177/0956797617708288