
# DummyAI Environment Setup

This repository contains the environment setup for `DummyAI`, a Python environment designed for Machine Learning and Deep Learning tasks. The environment includes popular libraries such as TensorFlow, Scikit-learn, XGBoost, and more, along with CUDA and cuDNN support for GPU acceleration.

## Requirements

- Anaconda or Miniconda installed on your system.

## Creating the Environment

To create the `DummyAI` environment using the provided `DummyAI.yaml` file, follow these steps:

1. **Clone the Repository** (if applicable):

   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```

2. **Create the Environment**:

   Run the following command to create the environment from the YAML file:

   ```bash
   conda env create -f DummyAI.yaml
   ```

   This command will create a new Conda environment named `DummyAI` with all the specified dependencies.

3. **Activate the Environment**:

   After the environment is created, activate it using the command:

   ```bash
   conda activate DummyAI
   ```

4. **Verify the Installation**:

   To ensure that everything is set up correctly, you can check the installed packages:

   ```bash
   conda list
   ```

## Included Packages

The environment includes the following key packages:

- **Python 3.8**: The programming language.
- **Jupyter Notebook**: For creating and sharing documents that contain live code, equations, visualizations, and explanatory text.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Support for large multi-dimensional arrays and matrices.
- **Scikit-learn**: Machine learning library.
- **Matplotlib & Seaborn**: Visualization libraries.
- **XGBoost**: Gradient boosting library.
- **CUDA Toolkit 11.2 & cuDNN 8.1.0**: For GPU acceleration (NVIDIA GPUs).
- **TensorFlow (<2.11)**: Deep learning framework.
- **TQDM**: A fast, extensible progress bar for loops.

## Notes

- Ensure that your system has a compatible NVIDIA GPU for CUDA and cuDNN to work correctly.
- The TensorFlow version is pinned to be less than 2.11 to ensure compatibility with other dependencies and custom requirements.

## Updating the Environment

If you need to update the environment with additional packages, you can modify the `DummyAI.yaml` file and run:

```bash
conda env update --file DummyAI.yaml --prune
```

## Deactivating the Environment

To deactivate the environment, use:

```bash
conda deactivate
```

## Removing the Environment

If you need to remove the environment, use:

```bash
conda env remove -n DummyAI
```

---

Feel free to modify the environment file as needed for your project requirements.
