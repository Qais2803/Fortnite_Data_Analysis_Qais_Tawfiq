# Fortnite_Data_Analysis_Qais_Tawfiq
Qais_Tawfiq_12144412


Executive Summary
This report presents a comprehensive analysis of a student project focused on analyzing player behavior and performance in Fortnite through data analytics and machine learning. Using a dataset titled "Fortnite Statistics.csv", the student implemented a game-focused analytics workflow involving data cleaning, visualization, clustering, and classification. The project’s key findings include identification of distinct player behavior clusters and a predictive model to classify high-performing players. Insights from the analysis can inform game design improvements and personalized player feedback systems.
Introduction
Online multiplayer games like Fortnite generate extensive data from player interactions, offering opportunities for data-driven insights. This project aims to harness that data to:
•	Understand player behavior patterns
•	Develop a predictive model for high performance
•	Inform potential game design improvements
The overarching goal was to combine exploratory data analysis with machine learning techniques to identify patterns and derive actionable insights.
Methodology
Game Design Choices and Rationale
The dataset reflects key performance metrics relevant to gameplay, such as Eliminations, Accuracy, Damage to Players, and Distance Traveled. These features align with core competencies in Fortnite, making them suitable for behavioral segmentation and performance evaluation.
Data Collection Approach
The student utilized a CSV file containing anonymized match statistics. The data was loaded into a pandas DataFrame and cleaned. For example, the Accuracy column was stripped of percentage signs and converted to float to enable numerical computations.
Analytics Dashboard Implementation
Using seaborn and matplotlib, the student constructed visualizations such as histograms and scatter plots. These included:
•	A histogram displaying the distribution of eliminations
•	A scatter plot showing the relationship between accuracy and damage dealt
These visuals helped in understanding player tendencies and correlations between performance variables.
Machine Learning Algorithm Selection and Implementation
Two ML approaches were used:
•	KMeans Clustering: Applied on normalized features (Eliminations, Accuracy, Damage to Players, Distance Traveled) to identify behavior-based player clusters.
•	Decision Tree Classification: Targeting a binary classification of players into high or low performers based on whether they achieved at least 3 eliminations. The model used features like Accuracy, Damage to Players, and Distance Traveled, and was trained using a 70/30 train-test split.
Results and Analysis
Key Patterns Discovered in Player Behavior
The KMeans clustering identified three distinct player groups:
1.	Low eliminations, low damage
2.	Moderate performance with decent accuracy
3.	High eliminations and high damage, potentially elite players
Machine Learning Insights and Their Accuracy
The Decision Tree classifier achieved reasonable performance, providing interpretable rules for identifying high performers. The classification report included precision, recall, and F1-score, indicating a balanced model fit.
Visualizations with Explanations
•	Histogram of Eliminations: Revealed that most players achieved few eliminations per game.
•	Scatter Plot (Accuracy vs Damage): Suggested a moderate correlation; higher accuracy tends to result in more damage.
•	Cluster Plot: Clearly showed group differentiation based on performance metrics.
•	Decision Tree Diagram: Illustrated decision paths for predicting high performers, enhancing interpretability.
Design Recommendations Based on Findings
•	Players in the low-performance cluster may benefit from in-game training or adaptive difficulty.
•	Accuracy could be a key metric for progression tracking or performance bonuses.
•	Machine learning insights can inform personalized coaching systems within the game.
Technical Challenges
Several technical hurdles were noted and addressed:
•	Data Cleaning: The Accuracy column required conversion from string percentage format to float.
•	Model Interpretability: While KMeans offers clustering, it lacks interpretability, which was addressed using Decision Trees for clearer rules.
•	Feature Scaling: KMeans performance improved after using StandardScaler to normalize features.
Future Improvements
•	Include additional metrics like player rank, kill/death ratio, or match duration.
•	Use advanced models (e.g., Random Forest, SVM) to compare classification performance.
•	Integrate real-time dashboards using tools like Dash or Streamlit.
•	Explore time-series analysis if temporal match data is available.
Conclusion
This project successfully demonstrates how game analytics and machine learning can yield actionable insights into player behavior. The student effectively cleaned, analyzed, and modeled the data, leading to meaningful performance categorizations and predictive capabilities. Key lessons include the value of feature engineering, the trade-off between model accuracy and interpretability, and the importance of visual storytelling in analytics.
References
•	Pedregosa et al. (2011). Scikit-learn: Machine Learning in Python. Journal of Machine Learning Research.
•	Seaborn Documentation. https://seaborn.pydata.org/
•	Matplotlib Documentation. https://matplotlib.org/
•	Fortnite Official Stats Guide. https://www.epicgames.com/fortnite/en-US/news
•	KMeans and DecisionTreeClassifier APIs – scikit-learn documentation


