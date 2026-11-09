# AIML Journey

> My personal log of learning Artificial Intelligence and Machine
> Learning --- concepts, implementations, experiments, debugging notes,
> and projects.

This repository documents my progress as I learn AIML practically and
build a stronger understanding of the mathematics behind the models. It
is also where I practise Git and GitHub.


------------------------------------------------------------------------

## Learning progress

### Covered / implemented

#### Python and data handling

-   [x] Python fundamentals for data science
-   [x] NumPy fundamentals and array operations
-   [x] pandas: loading, inspecting, selecting, and working with
    DataFrames
-   [x] Basic data cleaning and preprocessing
-   [x] Train/test splitting
-   [x] Handling missing values and scaling in an ML workflow
-   [x] Saving and loading data using Parquet
-   [x] Basic statistical exploration and correlation

#### Machine Learning

-   [x] Linear Regression
    -   Implemented a Linear Regression model.
    -   Worked with prediction and model evaluation.
    -   Practised MAE, RMSE, and R².
-   [x] Logistic Regression
    -   Implemented a Logistic Regression model.
    -   Applied it to a Student Pass Predictor.
-   [x] Student Score / Marks Prediction
    -   Worked with student-score data and a regression workflow.
-   [x] Student Pass Prediction
    -   Worked with student data and a classification workflow.

#### Neural Networks

-   [x] Started implementing a neural network using NumPy.
-   [x] Worked with the MNIST digit dataset.
-   [x] Studied the basic structure of a neural network: weights,
    biases, layers, and activations.

### Currently learning

-   [ ] Decision Trees
-   [ ] Random Forests
-   [ ] Neural Networks from scratch using NumPy
    -   [ ] Forward propagation
    -   [ ] Activation functions and loss calculation
    -   [ ] Gradients and the chain rule
    -   [ ] Backpropagation (mathematical understanding)
    -   [ ] Gradient descent and training loop
    -   [ ] Train and evaluate the MNIST classifier

### To be covered

This is the remaining topic list for my AIML foundations. I will update
the checklist as I learn each topic.

#### Machine Learning foundations

-   [ ] Complete Decision Trees and Random Forests
-   [ ] Bias--variance trade-off
-   [ ] Underfitting and overfitting
-   [ ] Cross-validation
-   [ ] Feature engineering and feature selection
-   [ ] Hyperparameter tuning
-   [ ] Classification metrics: confusion matrix, precision, recall,
    F1-score
-   [ ] Compare models and establish meaningful baselines

#### Deep Learning

-   [ ] Complete the NumPy neural network implementation
-   [ ] Understand backpropagation in depth
-   [ ] Learn PyTorch fundamentals
-   [ ] Tensors, autograd, and computational graphs
-   [ ] Build and train MLPs using PyTorch
-   [ ] Convolutional Neural Networks (CNNs)
-   [ ] Image classification projects

#### Further AIML topics

-   [ ] Natural Language Processing (NLP) fundamentals
-   [ ] Word representations and embeddings
-   [ ] Attention mechanism
-   [ ] Transformers
-   [ ] Large Language Models (LLMs)
-   [ ] Retrieval-Augmented Generation (RAG)
-   [ ] Model deployment and basic MLOps
-   [ ] Read and reproduce selected research papers

------------------------------------------------------------------------

## Projects and experiments

  -------------------------------------------------------------------------------
  Project / notebook              Area                    Status
  ------------------------------- ----------------------- -----------------------
  `linear.ipynb`                  Linear Regression       Implemented /
                                                          revisiting

  `linear/student_marks.ipynb`    Student marks / score   Implemented
                                  prediction              

  `linear/car_price.ipynb`        Car price prediction    Experiment

  `logistic.ipynb`                Logistic Regression     Implemented

  `logistic/student_pass.ipynb`   Student Pass Predictor  Implemented

  `dsnT_ranF.ipynb`               Decision Trees / Random In progress
                                  Forests                 

  `nn/digit.ipynb`                Neural Network using    In progress
                                  NumPy / MNIST           
  -------------------------------------------------------------------------------

The status describes the work visible in this repository and my learning
notes. I will add links, results, and explanations as each project
becomes more complete.

------------------------------------------------------------------------

## Repository structure

This is the current folder and file organisation, based on my local AIML
workspace. Some datasets and generated files are kept locally for
experiments.

``` text
AIML/
│
├── README.md
│
├── nn/
│   ├── digit.ipynb
│   └── mnist_train.csv
│
├── logistic/
│   ├── student_pass.ipynb
│   └── student-mat.csv
│
├── linear/
│   ├── output/
│   ├── car_price.ipynb
│   ├── CAR-DETAILS-FROM-CAR-DEKHO.csv
│   ├── student_scores.csv
│   └── student_marks.ipynb
│
├── dsnT_ranF.ipynb
├── logistic.ipynb
├── linear.ipynb
│
├── medical-charges.csv
├── weatherAUS.csv
├── aussie_rain.joblib
│
├── train_inputs.parquet
├── val_inputs.parquet
├── test_inputs.parquet
├── train_targets.parquet
├── val_targets.parquet
└── test_targets.parquet
```

*Note: This tree reflects the screenshots of my current workspace. The
exact contents may change as I organise experiments into folders.*

------------------------------------------------------------------------

## Tools and technologies

-   **Language:** Python
-   **Data work:** NumPy, pandas
-   **Visualisation:** Matplotlib
-   **Machine Learning:** scikit-learn
-   **Environment:** Jupyter Notebook
-   **Version control:** Git and GitHub
-   **Currently exploring:** neural networks with NumPy

------------------------------------------------------------------------

## Git and GitHub practice

I am learning Git alongside AIML and using this repository to practise a
clean version-control workflow.

``` bash
# Check repository status
git status

# Stage selected changes
git add <file>

# Review staged changes
git diff --staged

# Commit changes
git commit -m "Describe what changed"

# View commit history
git log --oneline --graph

# Push commits to GitHub
git push
```

Things I am practising: - \[ \] Working tree, staging area, and
commits - \[ \] Writing clear commit messages - \[ \] `.gitignore` and
ignored vs. tracked files - \[ \] Branches and merging - \[ \] Fetch,
pull, and push - \[ \] Resolving merge conflicts - \[ \] Undoing changes
safely with `restore`, `reset`, and `revert` - \[ \] Handling large
files and understanding Git LFS

### Dataset handling

Large datasets should generally not be committed directly to Git. I keep
local datasets available for my notebooks and exclude them from normal
Git commits when appropriate.

Example `.gitignore` entries (adjust these paths to match the files I
want to keep locally):

``` gitignore
# Datasets
nn/mnist_train.csv
nn/mnist_test.csv
linear/output/
*.parquet
*.joblib

# Python
__pycache__/
*.py[cod]
.venv/

# Jupyter
.ipynb_checkpoints/

# macOS
.DS_Store
```


------------------------------------------------------------------------

## Experiment log template

I will use this template when documenting a new model or experiment:

``` text
### Experiment: <name>

- Goal:
- Dataset:
- Concepts:
- Preprocessing:
- Model:
- Experiments:
- Evaluation metrics:
- Results:
- What I understood:
- Problems / debugging:
- What I need to improve:
- Next step:
```

------------------------------------------------------------------------

## Learning approach

For each topic, my goal is to:

1.  Understand the concept and the mathematics behind it.
2.  Implement it and inspect how it works.
3.  Experiment with data, parameters, and model behaviour.
4.  Evaluate the result using appropriate metrics.
5.  Record mistakes, observations, and limitations.
6.  Keep the code and Git history organised.

> **Learn the concept → implement it → experiment → evaluate → document
> → improve.**

This repository will grow as my understanding of AIML grows.
