# EDA Part 2 - Correlation & Data Storytelling:
### Week 2 - Day 5:

**What I did today:**

For this part, I switched to a different dataset - the Heart Disease
dataset - instead of reusing Titanic again. The goal was to go beyond
looking at one variable at a time (like I did on Day 4) and start looking
at relationships between variables, then wrap everything into a full,
narrated EDA notebook.

**Dataset used:** Heart Disease dataset (data/heart.csv)

**Here's what I worked through:**

1. Made a scatter plot of age vs cholesterol (chol) to check if there's any visible relationship between them.

2. Made grouped boxplots to compare:
   - max heart rate (thalch) across patients with vs without heart disease (target).
   - resting blood pressure (trestbps) across patients with vs without heart disease.

3. Computed the full correlation matrix for the numeric columns and visualized it as an annotated heatmap, which made it much easier to scan all the relationships at once instead of comparing columns one by one.

4. Picked out the strongest relationships and thought about what they might mean:
   - thalach (max heart rate) has a noticeable positive relationship with target - this could be a strong feature for a future classification model.
   - age and thalach are negatively related, which makes physiological sense - max heart rate tends to drop as people get older.
   - exang (exercise-induced angina) also showed a relationship with target, though I made sure to note that correlation doesn't mean causation here, especially with medical data.

5. Put everything together into one notebook that combines statistics, univariate analysis, outlier handling, bivariate analysis and correlation - with Markdown notes explaining what each part shows.

Tools used:
Seaborn, Pandas, Matplotlib, Jupyter Notebook

What I took away from this:
Switching datasets for this part actually helped - it forced me to think
about what the columns mean instead of just repeating steps from memory.
It also reminded me to be extra careful with causal language when working
with health-related data - a strong correlation is a starting point for
a hypothesis, not proof of a cause.