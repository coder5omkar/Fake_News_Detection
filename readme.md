📘 Fake News Identification
🎯 Goal
The primary objective of this project is to build a semantic-based classification system that can effectively differentiate between authentic and misleading news articles. By utilizing Word2Vec embeddings, the project focuses on capturing the underlying meanings of the text, which are then analyzed using supervised learning algorithms for classification.

🏢 Real-World Relevance
With the increasing circulation of fabricated news, there's a growing need for intelligent tools that can automatically detect misinformation. This solution showcases how semantic analysis can assist digital platforms and end users in evaluating the trustworthiness of online content.

🗂️ Data Overview
The dataset includes two distinct CSV files:

🔹 True.csv – Contains 21,417 samples of verified news articles.

🔹 Fake.csv – Contains 23,502 samples of fabricated news stories.

Each record provides:

📌 title: Headline of the news item

📌 text: Full article content

📌 date: Date when the article was published

📊 Key Observations
✅ Authentic Articles: Use formal language, topic-relevant vocabulary, and a coherent structure.

⚠️ False Articles: Tend to feature emotionally loaded words, recurring phrases, and a less organized layout. Certain word patterns and expressions are common in deceptive content.

📈 Visual analyses (like word clouds) confirmed noticeable differences in vocabulary usage between the two categories.

🔧 Workflow Breakdown
🧹 Data Preprocessing
🔹 Removal of noise and irrelevant characters

🔹 Lemmatization to unify word forms

🔹 Focused on extracting nouns via part-of-speech tagging to enhance semantic feature quality

🧠 Feature Construction
🔹 Employed pre-trained Word2Vec vectors to encode textual data into dense, meaning-rich formats

🧪 Classification Models
🔹 Logistic Regression

🔹 Decision Tree

🔹 Random Forest

📐 Performance Metrics
📊 Accuracy on Validation Set: 86.00%

📊 Precision: 85.90%

📊 Recall: 87.01%

📊 F1-Score: 86.45%

📄 Evaluation Summary
Class	Precision	Recall	F1-Score	Support
0 (Fake)	0.86	0.85	0.86	73
1 (Real)	0.86	0.87	0.86	77
Overall	0.86	0.86	0.86	150

Macro Average: Precision = 0.86, Recall = 0.86, F1 = 0.86

Weighted Average: Precision = 0.86, Recall = 0.86, F1 = 0.86

🔍 Insights
🔹 Semantic techniques enhance classification performance and reduce noise.

🔹 Pre-trained Word2Vec simplifies feature engineering while improving depth of analysis.

🔹 Random Forest consistently outperformed other models in accuracy and F1-score.

🔹 This approach provides a practical foundation for scalable misinformation detection tools.

🔮 Enhancements Ahead
🔹 Adapt Word2Vec embeddings using domain-specific datasets for improved relevance.

🔹 Explore context-aware models like BERT to further capture linguistic nuances and dependencies.

