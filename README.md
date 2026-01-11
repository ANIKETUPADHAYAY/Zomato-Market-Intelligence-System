Zomato Market Intelligence: Advanced Cuisine Clustering & Recommendation Framework
🎯 Project Overview
This repository contains an end-to-end Unsupervised Machine Learning pipeline designed to analyze over 10,000 restaurant data points. By leveraging Natural Language Processing (NLP) and K-Means Clustering, this project identifies latent patterns in culinary offerings and customer sentiment to drive high-precision restaurant recommendations.

Key Engineering Highlights:
Feature Engineering: Transformed raw restaurant metadata into a structured feature space, handling high-cardinality categorical data (Cuisines, Localities).

NLP Engine: Processed 10k+ user reviews using TF-IDF vectorization to extract sentiment-weighted keywords for more accurate clustering.

Optimal Clustering: Utilized the Elbow Method and Silhouette Analysis to mathematically determine the most stable restaurant segments.

Dimensionality Reduction: Implemented PCA to visualize complex, multi-dimensional culinary data in a 2D interpretable space.

🛠️ Technical Architecture
The pipeline follows a standard MLOps lifecycle to ensure the model is production-ready:

Data Ingestion: Cleaning and merging Restaurant Metadata with User Reviews.

Preprocessing: Custom Regex for text cleaning, handling missing values, and feature scaling.

Modeling: Iterative K-Means testing to group restaurants based on cost, cuisine diversity, and user ratings.

Inference: Providing a framework to recommend restaurants within the same "cluster" based on user preferences.

📊 Business Impact & Use Cases
Market Gap Analysis: Identified underserved "budget-friendly" clusters in high-density areas.

Personalized Marketing: Enables platforms to target users with specific "Culinary Personas" (e.g., "The Premium Explorer" vs "The Value Foodie").

Growth Strategy: Provides data-backed evidence for new restaurant entries based on cluster saturation levels.

📁 Project Structure
Plaintext

├── data/
│   ├── metadata_v1.csv           # Business attributes
│   └── reviews_v1.csv            # User sentiment data
├── notebooks/
│   └── architecture_final.ipynb  # Main clustering pipeline
├── src/
│   └── utils.py                  # Helper functions for text cleaning
└── requirements.txt              # Production dependencies
🚀 Future Roadmap
Real-time Streaming: Integrate Kafka to update clusters as new reviews arrive.

Deployment: Wrap the recommendation engine in a FastAPI container for production use.

LLM Integration: Use LangChain to summarize review sentiments within each cluster.
