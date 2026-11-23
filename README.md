# Tree-Based Models: Random Forests

## Objective
I compared a random forest with a single decision tree, OLS and Ridge on California Housing, and checked how the forest ranks its features.

## Methodology
- Split California Housing into training and test rows (80/20).
- Fit a single decision tree, OLS, Ridge and a random forest, and compared their test R².
- Compared impurity (MDI) and permutation importance for the forest.
- Tuned max_depth and max_features with 3-fold cross-validation.
- Wrote my own prompt asking an AI for a feature-importance chart function, and checked its output against my own numbers.

## Key Findings
- Test R²: 0.6228 for the single tree, 0.5758 for Ridge and 0.8046 for the random forest.
- Latitude scored 0.0890 by MDI but 0.4427 by permutation importance.
- The tuned forest reached a test R² of 0.8094.
- The AI's function took 2 rounds, and every value matched my permutation importance numbers in every printed digit.****
