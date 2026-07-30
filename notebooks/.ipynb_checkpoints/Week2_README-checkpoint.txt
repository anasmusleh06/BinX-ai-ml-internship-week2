# Week 2 - Math Foundations & EDA

## BinX Tech - AI & ML Internship Program

**Overview:**
This week was about building the math foundations that ML models rest on - descriptive statistics, probability, and linear algebra - and then putting that understanding to work through a full Exploratory Data Analysis (EDA) on real datasets.

**Day-by-day summary:**

Day 1 - Descriptive Statistics
- Learned mean, median, mode, variance, standard deviation, and IQR.
- Practiced choosing the right measure of central tendency depending on whether the data has outliers or not (e.g. median over mean for skewed data).

Day 2 - Probability & Distributions
- Covered the core probability rules (complement, addition, multiplication), conditional probability, and Bayes' theorem.
- Simulated coin flips and sampled from a normal distribution to connect the theory with actual code.

Day 3 - Linear Algebra for ML
- Represented data samples as vectors and datasets as matrices.
- Computed dot products and matrix multiplications, and connected them directly to how a linear model actually produces a prediction.
Day 4 - EDA Part 1: Distributions & Outliers
- Used the Titanic dataset.
- Performed univariate analysis with histograms, boxplots, and countplots.
- Applied the IQR method to detect outliers in the Fare column and decided to keep them since they reflected real first-class fares, not data errors.
- Noticed class imbalance in Pclass and Sex.

Day 5 - EDA Part 2: Correlation & Data Storytelling
- Switched to the Heart Disease dataset to practice EDA on a different kind of data instead of repeating Titanic.
- Performed bivariate analysis with scatter plots and grouped boxplots.
- Computed a correlation matrix and visualized it as a heatmap.
- Identified the strongest relationships (thalach vs target, age vs thalach) and reasoned about what they might mean, while being careful not to confuse correlation with causation.

Datasets used this week:
- Titanic dataset (data/train.csv) - Days 1-4
- Heart Disease dataset (data/heart.csv) - Day 5

Tools used:
NumPy, Pandas, Matplotlib, Seaborn, Jupyter Notebook, Git & GitHub

Overall takeaway:
The math this week wasn't taught as theory for its own sake - every
concept tied directly into how EDA and ML models work in practice.
Switching to a second dataset for Day 5 was useful because it pushed me
to actually reason about new columns instead of just repeating steps I
already knew from Titanic. The biggest lesson from the whole week: an
outlier or a correlation is a question to investigate, not an automatic
answer.