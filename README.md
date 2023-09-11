# ECON526 - Fall 2023

This is a MA-level course in quantitative economics, data science, and causal inference in economics.


This course will have a combination of coding, theory, and development of mathematical background.  All coding is done in Python.

# Course materials
- Get a [GitHub](www.github.com) ID and apply for the [Student Developer Pack](https://education.github.com/pack) to get further free features
- Consider clicking `Watch` at the top of this repository to see file changes

All materials will be on github, and canvas will be used to submit assignments/communication.

There is no assigned physical textbook, but we will be using lecture notes from:
- [Causal Inference for The Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html)
- [QuantEcon Python and Data Science Lectures](https://quantecon.org/projects/#filter=lecture)

# Computing Environment
While you can use the [UBC JupyterOpen](https://open.jupyter.ubc.ca/) for this course, we strongly suggest installing Python on your local machine.  The easiest way to do this is:
- Install [Anaconda](https://www.anaconda.com/download) to install python and its packages for your operating system
- Install [git](https://git-scm.com/downloads) for your operating system
- Optionally: install (a) [Github Desktop](https://desktop.github.com/); (b) [VS Code](https://code.visualstudio.com/) to make it easier to manage downloaded notebooks.
- Then clone the following repositories onto your local machine using a terminal, using either git directly (e.g. in terminal go `git clone https://github.com/ubcecon/ECON526.git`), [GitHub Desktop](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop), or [VS Code](https://code.visualstudio.com/docs/sourcecontrol/intro-to-git#_clone-a-repository-locally)
    - https://github.com/ubcecon/ECON526
    - https://github.com/QuantEcon/lecture-python-intro.notebooks
    - https://github.com/QuantEcon/lecture-python.notebooks
    - https://github.com/QuantEcon/lecture-datascience.notebooks
    - In some cases you will need to manually install packages (by doing `pip install -r requirements.txt` within some of those repositories, or manually installing packages as required)

For introductory users, we recommend using [GitHub Desktop](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop) which allows cloning from a button on the public github repo directly.  For intermediate users, we recommend skipping the GitHub Desktop and instead using [VS Code](https://code.visualstudio.com/docs/sourcecontrol/intro-to-git#_clone-a-repository-locally) since you will likely begin using the VSCode editor as your primary Python (and latex) editor sooner than later.

## Syllabus
See [Syllabus](syllabus.md) for more details

## Problem Sets and Exams

The course has two midterms, weekly to bi-weekly problem sets, and a final data project due the last day of class.

1. **September 10th Midnight:** [Problem Set 1](problem_sets/problem_set_1.ipynb)
2. **September 17th Midnight:** [Problem Set 2](problem_sets/problem_set_2.ipynb)
3. **October 11th:** IN CLASS MIDTERM #1
4. **November 8th:** IN CLASS MIDTERM #2
5. **December 8th Midnight:** Data Project Due

See the `/problem_sets` folder within this repository for the problem sets as jupyter notebooks.  You should modify them directly as Jupyter notebooks, and the TA will explain how to submit them.

## Lectures
This year the course will be taught in three parts where the later parts of the course will follow material in [Causal Inference for The Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html).

This lecture begins assuming you have completed the math/programming bootcamp for our masters students, or had an existing python-based programming course.  To refresh your knowledge, see basics in [QuantEcon Data Science Lectures](https://datascience.quantecon.org/) or [QuantEcon Python Programming for Economics and Finance](https://python-programming.quantecon.org/intro.html).

### Jesse

- **September 6**: Introduction to Numerical Linear Algebra and its Applications in Data Science
   - **Topics:** Overview of computational complexity and numerical precision, solving systems of equations, geometric interpretations of linear algebra, matrix decompositions, linear least squares, and eigenvalues and eigenvectors.  Preparation for applications.
   - **Material:** 
     - [Linear Algebra Foundations Slides](lectures/linear_algebra_foundations.pdf) (as [Jupyter Notebook](lectures/linear_algebra_foundations.ipynb))
   - **Self-study:**
     - Basics of linear algebra, matrices, norms, and linear independence: https://python.quantecon.org/linear_algebra.html
     - Numerical optimization: https://datascience.quantecon.org/scientific/optimization.html
     - Systems of Equations: https://python.quantecon.org/linear_algebra.html#solving-systems-of-equations
     - Eigenvectors and eigenvalues: https://python.quantecon.org/linear_algebra.html#eigenvalues-and-eigenvectors
     - Downloading and manipulating data in Python: https://intro.quantecon.org/long_run_growth.html and https://intro.quantecon.org/business_cycle.html
   - **(Optional) Extra Material**:
     - Introductory material on linear algebra: https://intro.quantecon.org/linear_equations.html and https://datascience.quantecon.org/scientific/applied_linalg.html
     - Matrix decompositions and other topics: https://python.quantecon.org/linear_algebra.html#further-topics

- **September 11**: Applications of Linear Algebra (Eigenvalues)
   - **Topics:** Geometric series and present values, difference equations, steady states, and convergence, unemployment dynamics, present discounted values
   - **Material:** 
     - Finishing off [Linear Algebra Foundations Slides](lectures/linear_algebra_foundations.pdf)
     - [Linear Algebra Applications Slides](lectures/linear_algebra_applications.pdf) (as [Jupyter Notebook](lectures/linear_algebra_applications.ipynb))
   - **Self-study:**
     - Geometric Series and Present Values: https://intro.quantecon.org/geom_series.html#example-interest-rates-and-present-values
     - Portfolio example: https://datascience.quantecon.org/scientific/applied_linalg.html#portfolios
     - Unemployment Dynamics example: https://datascience.quantecon.org/scientific/applied_linalg.html#unemployment-dynamics
   - **(Optional) Extra Material**:
     - Supply and Demand: https://intro.quantecon.org/intro_supply_demand.html
     - More on Competitive Equilibrium: https://intro.quantecon.org/supply_demand_multiple_goods.html

- **September 13**: Applications of Linear Algebra (Latent Variables)
   - **Topics:** Latent variables and principle components, k-means clustering, and valuing portfolios
   - **Material:** 
     - [Linear Algebra Applications Slides](lectures/linear_algebra_applications.pdf) (as [Jupyter Notebook](lectures/linear_algebra_applications.ipynb))
   - **Self-study:**
     - [scikit-learn k-means docs](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
     - [scikit-learn PCA docs](https://scikit-learn.org/stable/modules/decomposition.html#principal-component-analysis-pca)
     - [seaborn tutorials](https://seaborn.pydata.org/tutorial/introduction.html)
<!--
   - **Material:**
     - Solow-Swan Growth Model: https://intro.quantecon.org/solow.html
     - Nonlinear Dynamics and Stability: https://intro.quantecon.org/scalar_dynam.html
     - Eigenvalues and stability of linear systems
   - **(Optional) Extra Material**:
     - More on the Solow Model and Python: https://python-programming.quantecon.org/python_oop.html#example-the-solow-growth-model

-->
<!--   
   - **Material:**
     - https://intro.quantecon.org/prob_dist.html
     - https://python.quantecon.org/prob_meaning.html
     - Axioms of probability, conditional expectations, Bayes' rule, Law of Iterated Expectations
   - **(Optional) Extra Material**:
     - https://python.quantecon.org/prob_matrix.html
-->
- **September 18**: Dynamics and the Solow-Swan Model
<!--
   - **Material:**
     - https://python.quantecon.org/lln_clt.html
     - https://intro.quantecon.org/inequality.html
   - **(Optional) Extra Material**:
     - https://datascience.quantecon.org/scientific/randomness.html     
-->
- **September 20**: Probability
<!--
   - **Material:**
     - https://intro.quantecon.org/markov_chains_I.html
     - https://intro.quantecon.org/lake_model.html
   - **(Optional) Extra Material**:
     - https://intro.quantecon.org/markov_chains_II.html
     - https://datascience.quantecon.org/scientific/randomness.html#loan-states
     - https://python.quantecon.org/finite_markov.html
-->
    
- **September 25**: Simulating Randomness and Stochastic Processes
    <!--Introduction to Deep Learning (time-permitting)
    -->    

-  **September 27**: Causality, Treatment and Potential Outcomes
    - **Material:**
       - https://matheusfacure.github.io/python-causality-handbook/01-Introduction-To-Causality.html
       - https://matheusfacure.github.io/python-causality-handbook/02-Randomised-Experiments.html
-  **October 2 (Statutory holiday)**

-  **October 4**: Graphical Causal Models and Confounders
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/04-Graphical-Causal-Models.html

-  **October 9 (Statutory holiday)**

-  **October 11**
    - **IN CLASS MIDTERM #1**
### Phil
-   **October 12** ("Make-up Monday") Linear Regression, Omitted Variable Bias
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/05-The-Unreasonable-Effectiveness-of-Linear-Regression.html

-   **October 16** Groups and Dummy Regression
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/06-Grouped-and-Dummy-Regression.html
-   **October 18** Beyond Confounders - Good and Bad Controls, Selection Bias
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/07-Beyond-Confounders.html
-   **October 23** Instrumental Variables
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/08-Instrumental-Variables.html
-   **October 25** Matching
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/10-Matching.html
-   **October 30** Propensity Scores
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/11-Propensity-Score.html
-   **November 1**: Doubly Robust Estimation
    - **Material:**
      - https://matheusfacure.github.io/python-causality-handbook/12-Doubly-Robust-Estimation.html
### Paul

-    **November 6**: Overview and begin difference in differences
    - https://matheusfacure.github.io/python-causality-handbook/13-Difference-in-Differences.html
-  **November 8**
    - **IN CLASS MIDTERM #2**
-  **November 10**: Difference in Differences
    - https://matheusfacure.github.io/python-causality-handbook/13-Difference-in-Differences.html
-  **November 13 (Midterm Break)**
-  **November 15 (Midterm Break)**
-  **November 20**: Panel Data and Fixed Effects
    - https://matheusfacure.github.io/python-causality-handbook/14-Panel-Data-and-Fixed-Effects.html
-  **November 22**: The Difference in Differences Saga
    - https://matheusfacure.github.io/python-causality-handbook/24-The-Diff-in-Diff-Saga.html
-  **November 27**: Synthetic Control
    - https://matheusfacure.github.io/python-causality-handbook/15-Synthetic-Control.html
    - https://matheusfacure.github.io/python-causality-handbook/25-Synthetic-Diff-in-Diff.html
-  **November 29**: Predictive Models
    - https://matheusfacure.github.io/python-causality-handbook/17-Predictive-Models-101.html
    - https://datascience.quantecon.org/tools/regression.html
- **December 4**: Debiased/Orthogonal Machine Learning
    - https://matheusfacure.github.io/python-causality-handbook/22-Debiased-Orthogonal-Machine-Learning.html
    - https://datascience.quantecon.org/applications/ml_in_economics.html#estimation-of-nuisance-functions    -
- **December 6**: Regression Discontinuity
    - https://matheusfacure.github.io/python-causality-handbook/16-Regression-Discontinuity-Design.html
- **December 8**
    - **DATA PROJECT DUE**
