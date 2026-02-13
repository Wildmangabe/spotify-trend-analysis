# Global Spotify Trends: Regional & Temporal Data Mining Analysis
**Authors:** Maya Shah and Gabe Wild

---

## Project Overview
This project deconstructs global music consumption patterns on Spotify from 2017 to 2021. By merging massive daily chart datasets with specific audio features, we identified distinct "music profiles" using unsupervised machine learning and investigated how regional preferences shift across 60+ countries over time.

## Key Features & Methodology
* **Data Integration:** Processed over 26 million rows of Spotify Top 200 daily charts and mapped them to high-dimensional audio feature data (danceability, energy, valence, etc.).
* **Clustering & Segmentation:** Applied **K-Means** and **DBSCAN** to group songs into representative "audio profiles."
* **Dimensionality Reduction:** Used **PCA**, **t-SNE**, and **UMAP** to visualize complex musical relationships in 2D and 3D space.
* **NLP for Metadata:** Leveraged **Word2Vec** to analyze and process textual metadata associated with global tracks.
* **Statistical Validation:** Performed **Pairwise Tukey HSD** tests and cosine similarity analysis to ensure the statistical significance of our discovered clusters.
* **Interactive Mapping:** Developed a global choropleth map using **Plotly** to visualize the dominance of specific music profiles by region.

## Technologies Used
- **Language:** Python
- **Libraries:** Pandas, NumPy, SciPy, Scikit-learn
- **ML/Manifold Learning:** UMAP-learn, HDBSCAN, Gensim (Word2Vec)
- **Visualization:** Plotly Express, Seaborn, Matplotlib

## Visualizing the Data
The project utilizes manifold learning to project high-dimensional audio data into a visualizable format, allowing us to see how different genres and styles cluster together based on mathematical similarity rather than just manual genre tags.

## Findings & Conclusions
Our analysis revealed that global music consumption is not a monolith; countries often belong to specific "audio profile" clusters that remain stable over long periods. These findings provide a data-driven explanation for the success of feature-driven recommendation engines (like Spotify’s "Discover Weekly"), as song similarity can be accurately mapped through objective audio features.
