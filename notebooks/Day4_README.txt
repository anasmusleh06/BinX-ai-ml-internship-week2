# EDA Part 1 - Distributions & Outliers:
### Week 2 - Day 4:

**What I did today:**

Today's focus was on EDA (Exploratory Data Analysis) - before jumping into any modeling, I had to actually understand the dataset first: how each column is distributed and whether there are any weird values I need to watch out for.

**Here's what I worked through:**

1. Loaded the dataset and plotted a histogram for every numeric column, just to get a feel for how each one is distributed (normal and skewed) - I used the Titanic dataset (train.csv) for this -.

2. Made boxplots for Age and Fare specifically, since these are the two columns most likely to have outliers. The boxplot made it easy to spot the median, the quartiles and any points sitting way outside the whiskers.

3. Used the IQR method on the Fare column to flag outliers with actual code instead of just eyeballing it. I found a good number of outliers, but after thinking about it, I decided not to remove them - the high Fare values make sense (first-class tickets cost a lot more), so they're real data, not mistakes.

4. Made countplots for Sex, Pclass and Embarked to check the balance of the categories. Noticed that Pclass is pretty imbalanced - a lot more third-class passengers than first or second class and Sex isn't perfectly balanced either.

**Tools used:**
Seaborn, Pandas, Matplotlib, Jupyter Notebook

**What I took away from this:**
An outlier isn't automatically "wrong" - it's something you have to actually investigate before deciding to keep it, cap it, or drop it. In this case, keeping the Fare outliers made more sense than removing them.