# Fairness Evaluation in Recommender Systems

This project investigates the fairness of recommender systems by implementing, evaluating, and comparing multiple collaborative filtering models on two real-world datasets: **MovieLens 100K** and **Yelp**.

We build three personalized recommendation models — **SVD++**, **UserKNN**, and **ItemKNN** — and evaluate them based on both **predictive accuracy (RMSE)** and a comprehensive set of **fairness metrics**. These metrics assess how the models treat users across sensitive attributes, focusing primarily on **gender**.

## Goals

- Implement and tune multiple recommendation algorithms
- Evaluate model performance using RMSE
- Assess fairness using both individual and group-level metrics
- Compare model behavior across datasets and demographic groups

## Datasets Used

- **MovieLens 100K**  
  Includes demographic information like age and gender. Used for all model training, testing, and fairness evaluation.
  
- **Yelp Open Dataset**  
  Used for fairness evaluation with gender as the only sensitive attribute available.

## Fairness Metrics Applied

- Counterfactual Difference  
- Consistency Score  
- Statistical Parity of Exposure  
- Rawlsian Maximin Exposure  
- Local Individual Fairness  
- Calibration Error  
- Disparate Impact Ratio  
- Demographic Parity

## Repository Structure
├── Yelp/ │ └── yelp_model_fairness.ipynb ├── Movielens/ │ ├── 01_EDA_and_Fairness_Metrics.ipynb │ ├── 02_SVDpp_Model.ipynb │ ├── 03_UserKNN_Model.ipynb │ ├── 04_ItemKNN_Model.ipynb │ └── data/ │ ├── archive.zip │ ├── movielens_data/ │ ├── df_full.csv │ ├── itemknn_predictions.csv │ ├── svdpp_predictions.csv │ └── userknn_predictions.csv ├── Literature_Review/ │ └── literature_review.md ├── Conclusion/ │ └── conclusion.md ├── README.md ├── .gitignore

## Requirements

- Python 3.8+
- Jupyter Notebook
- `pandas`, `numpy`, `scikit-learn`
- `surprise` (for SVD++)
- `matplotlib`, `seaborn`

## Authors

- Tim Zijlstra
- Lucas van der Wielen

## License

This project is licensed under the MIT License.
