# Cross_Val-vs-Train_Test

🚀 Train-Test Split vs Cross-Validation — When and Why? 🤔

In machine learning, choosing the right evaluation strategy can make or break your model's performance. Here’s a quick guide I explored in the notebook:
🔍 Train-Test Split
✅ Simple & fast (e.g., 80/20 or 70/30 split)
✅ Ideal for large datasets
❌ High variance on small or unbalanced data

📌 Use when:
• You need a quick performance check
• Your dataset is huge
• You're doing final evaluation before deployment

🔍 Cross-Validation (e.g., K-Fold)
✅ More robust and reliable
✅ Reduces variance by averaging multiple train/test combinations
❌ Takes more time/computation

📌 Use when:
• Dataset is small to medium
• You're comparing models
• You're tuning hyperparameters
• You want a stable and fair performance estimate

💡 In my GitHub notebook, I walk through real Python code using scikit-learn, showing how different strategies can influence your results — and how to avoid data leakage when applying scaling or encoding.

🎯 Purpose of the Notebook
To compare model performance using:
1. Train-Test Split
2. Cross-Validation

📦 Step-by-Step Code Summary
✅ 1. Imports & Dataset
✅ 2. EDA & Plotting
✅ 3. Train-Test Split Evaluation
 Result of using Train-Test Split
 
    🏆 Model Evaluation Complete 🏆 
╒════════════════════════╤════════════╕
│ Model                  │   Accuracy │
╞════════════════════════╪════════════╡
│ XGBClassifier          │       0.84 │
├────────────────────────┼────────────┤
│ LogisticRegression     │       0.82 │
├────────────────────────┼────────────┤
│ RandomForestClassifier │       0.82 │
├────────────────────────┼────────────┤
│ KNeighborsClassifier   │       0.7  │
├────────────────────────┼────────────┤
│ SVC                    │       0.69 │
╘════════════════════════╧════════════╛

✅ 4. Cross-Validation
 Result of using Train-Test Split

    🏆 Model Evaluation Complete 🏆 
╒════════════════════════╤════════════╕
│ Model                  │   Accuracy │
╞════════════════════════╪════════════╡
│ RandomForestClassifier │       0.84 │
├────────────────────────┼────────────┤
│ LogisticRegression     │       0.83 │
├────────────────────────┼────────────┤
│ SVC                    │       0.83 │
├────────────────────────┼────────────┤
│ XGBClassifier          │       0.79 │
├────────────────────────┼────────────┤
│ KNeighborsClassifier   │       0.64 │
╘════════════════════════╧════════════╛

🧠 Final Thought:
Using both methods together is a great way to:
• Compare evaluation strategies
• Avoid overfitting
• Choose the most trustworthy model
