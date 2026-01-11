**Zomato Market Intelligence: Advanced Cuisine Clustering & Recommendation Framework**

**🎯 Project Overview**
This repository contains an end-to-end Unsupervised Machine Learning pipeline designed to analyze over 10,000 restaurant data points. By leveraging Natural Language Processing (NLP) and K-Means Clustering, this project identifies latent patterns in culinary offerings and customer sentiment to drive high-precision restaurant recommendations.

**🚀Key Engineering Highlights**
Feature Engineering: Transformed raw restaurant metadata into a structured feature space, handling high-cardinality categorical data such as Cuisines and Localities.

NLP Engine: Processed 10k+ user reviews using TF-IDF Vectorization to extract sentiment-weighted keywords for increased clustering accuracy.

Optimal Clustering: Utilized the Elbow Method and Silhouette Analysis to mathematically determine the most stable and distinct restaurant segments.

Dimensionality Reduction: Implemented PCA (Principal Component Analysis) to visualize complex, multi-dimensional culinary data in a 2D interpretable space.

🛠️ Technical Architecture
The pipeline follows a standard MLOps lifecycle to ensure the model is production-ready:

Data Ingestion: Automated cleaning and merging of Restaurant Metadata with User Reviews.

Preprocessing: Utilized Custom Regex for text cleaning, handled missing values, and applied feature scaling.

Modeling: Performed iterative K-Means testing to group restaurants based on cost density, cuisine diversity, and user ratings.

Inference: Developed a framework to provide real-time recommendations within calculated clusters based on user input.

**📊 Business Impact & Use Cases**
Market Gap Analysis: Successfully identified underserved "budget-friendly" clusters in high-density urban areas.

Personalized Marketing: Enables platforms to target users with specific "Culinary Personas" (e.g., "The Premium Explorer" vs. "The Value Foodie").

Growth Strategy: Provides data-backed evidence for market entry based on cluster saturation levels.
