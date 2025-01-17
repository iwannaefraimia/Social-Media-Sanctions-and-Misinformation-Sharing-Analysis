# Social Media Sanctions and Misinformation Sharing  

## Description  
This project investigates the relationship between political orientation, misinformation sharing, and social media suspensions. The analysis evaluates whether social media sanctions are politically biased or result from differences in misinformation sharing across political beliefs. The goal is to determine if political orientation directly influences suspension or if other factors play a larger role.

## Dataset  
The analysis uses data provided in `mosleh_et_al_data.csv`. The dataset includes several independent variables related to political activity, misinformation, and user behavior on social media.

### Key Variables  
The following independent variables are normalized (z-scored) for the analysis:  
- **pc1_politics**: Political activity principal component 1.  
- **pc1_misinfo**: Misinformation principal component 1.  
- **pc1_fol**: Principal component related to follower dynamics.  
- **pc1_harmful_language**, **pc2_harmful_language**, **pc3_harmful_language**: Components representing harmful language.  
- **pc1_valence**: Sentiment valence.  
- **tweets_in_2wk**: Number of tweets in two weeks.  
- **botsentinel_score**: Score indicating bot-like behavior.  
- **extremity**: Measure of extremism in user behavior.  
- **w_moral_outrage**: Weighted moral outrage.  
- **liwc_political**: Linguistic indicator of political language.  
- **log_freq_pr_1h**: Log-transformed frequency of posting per hour.  
- **log_repeated_tweet_count**: Log-transformed count of repeated tweets.  
- **barbera_std**: Social network positioning based on Barbera's model.  
- **politics_sites1_std**, **politics_sites2_ideo_std**: Standardized scores of political website activity.  

## Analysis Steps  
1. **Data Preprocessing**  
   - Normalize independent variables using z-scores.  
   - Winsorize variables where necessary to handle outliers.  

2. **Regression Analysis**  
   - Perform probit regression to predict suspension using normalized independent variables.  
   - Apply Bonferroni and Holm-Bonferroni corrections to reduce Type I errors.  
   - Repeat the analysis using logit regression for comparison.  

3. **Results Interpretation**  
   - Evaluate whether political orientation influences suspension.  
   - Analyze the impact of misinformation and other variables on suspension likelihood.  

## Tools and Libraries  
- **Python**: Programming language used for analysis.  
- **pandas**: For data manipulation and preprocessing.  
- **numpy**: For numerical operations.  
- **statsmodels**: For regression analysis.  
- **scipy**: For statistical corrections.  
- **matplotlib**/**seaborn**: For visualizations.  

## Submission Instructions  
The submission includes:  
- A **Jupyter Notebook** documenting the code, analysis steps, and results.  
- All necessary files (e.g., `mosleh_et_al_data.csv`).  

### Key Features of the Notebook:  
- Fully replicable analysis.  
- Clear documentation for readers with basic Python knowledge.  
- User-friendly outputs with relevant columns and tables.  

## Academic Integrity  
This project adheres to the honor code for individual assignments. General help may be sought from online resources for Python usage but not for direct solutions to assignment questions.  

## References  
- Moshen Moshel et al., *Nature*: Research on social media sanctions and misinformation sharing.  
