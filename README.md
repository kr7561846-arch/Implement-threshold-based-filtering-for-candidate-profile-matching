🎯 The Mission
Searching for the right candidate in a sea of PDFs is a classic "needle in a haystack" problem. Recruiters are often buried under hundreds of documents where the perfect match is obscured by formatting noise or sheer volume.

I built this project to automate the heavy lifting of recruitment. Moving beyond rigid keyword searches, this tool leverages Natural Language Processing (NLP) and Machine Learning to "read" resumes, analyze the semantic DNA of a profile, and rank candidates based on their actual professional fit.

⚙️ How It Works: The Logic Flow
1. Semantic Understanding
Instead of simple word-matching, the system utilizes TF-IDF (Term Frequency-Inverse Document Frequency).

The Logic: It identifies the mathematical "weight" of a candidate's skills.

The Result: It recognizes that "Python" in a Data Science context is more significant than generic filler words, allowing the model to focus on high-value expertise.

2. Machine Learning Pipeline
Vectorization: Text data is converted into high-dimensional vectors.

Classification: A K-Nearest Neighbors (KNN) algorithm wrapped in a One-Vs-Rest Classifier categorizes resumes into professional domains.

Threshold-Based Filtering: The system calculates a similarity score for all 962 candidates, ranks the Top 100, and extracts the Top 20 "Elite" Matches for the final shortlist.

3. Performance & Accuracy
90% Precision: Validated through a rigorous Confusion Matrix analysis. The model accurately identifies the correct job category 9 out of 10 times.

Massive Efficiency: A task that would take a human recruiter ~22 hours (for 962 resumes) is completed by this engine in under 5 seconds.

📊 Why This Is a Game Changer
Instant Ranking: Immediate visibility of the Top 20 candidates.

Heat-Map Visualization: A data-driven dashboard using Green/Yellow/Red logic to communicate match intensity at a glance.

Bias Mitigation: By focusing on objective vectorized skill data, the system promotes a fairer initial screening process.

🛠️ Technical Snapshot
Dataset: 962 Rows of Professional Resume Data.

Key Algorithms: KNN (K-Nearest Neighbors), One-Vs-Rest Classifier, TF-IDF.

Evaluation Metrics: 90% Precision Score, Confusion Matrix, F1-Score.

Visualization: Seaborn Ranking Charts, Categorical Pie Distributions.
