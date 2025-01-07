# Green Skills Analysis Using AI and ESCO Taxonomy

This repository contains the code and resources for analyzing green skills in job postings using advanced AI techniques and the ESCO taxonomy. The project leverages embeddings, similarity search algorithms, and threshold optimization to identify and classify relevant skills, occupations, and industries from unstructured job description data.

## Key Features

- **Skill Extraction**: Automatically identifies the top 10 closest skills for each job posting using vector embeddings and cosine similarity.
- **Threshold Optimization**: Iterative process to determine the optimal similarity threshold for balancing precision, recall, and document retrieval rates.
- **Green Skills Classification**: Secondary step to filter and classify postings containing green skills, aligned with ESCO's taxonomy.
- **Occupation and Industry Mapping**: Maps job postings to standardized ESCO occupations and ISIC industries for structured classification.
- **Multi-Region Insights**: Methodology applied to datasets from Egypt, Kenya, and India, enabling cross-regional comparisons of green job trends.

## Technologies Used

- **AI and NLP**:
  - OpenAI embeddings for semantic similarity
  - LangChain framework for embedding-based retrieval
- **Data Management**:
  - Elasticsearch for similarity searches and vector storage
  - Python (Pandas, NumPy) for preprocessing and analysis
- **Visualization**:
  - Matplotlib and Seaborn for visualizing trends and results

## Repository Structure

```
green-skills-analysis/
├── data/              # datasets and preprocessing scripts (data is currently restricted due to confidentiality)
├── notebooks/         # Jupyter notebooks for exploratory analysis and methodology demonstration
├── README.md          # Project overview and instructions
```

## How to Use

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/green-skills-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd green-skills-analysis
   ```
3. Set up a virtual environment and install dependencies:
   ```bash
   python3 -m venv env
   source env/bin/activate
   pip install -r requirements.txt
   ```

### Running the Analysis

1. Preprocess datasets:
   - Place your job posting datasets in the `data/` folder.
   - Run the preprocessing script:
     ```bash
     python scripts/preprocess_data.py
     ```

2. Perform skill extraction and threshold optimization:
   ```bash
   python scripts/skill_extraction.py --threshold 0.7
   ```

3. Visualize results:
   - Use the `notebooks/` directory to explore trends and outputs interactively.

### Results and Outputs

- Extracted skills, occupations, and industries for job postings
- Visualizations of green job trends across regions and industries
- Logs documenting threshold optimization and retrieval counts

## Objectives

This project provides a scalable, reproducible framework for analyzing labor market data, with a focus on green jobs and skills. It is designed for use by researchers, policymakers, and industry professionals interested in sustainable development and workforce planning.

## Contributions

Contributions are welcome! Feel free to fork the repository, open issues, or submit pull requests to enhance the methodology or add new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This **`README.md`** provides a professional, detailed overview of your project, guiding users on setup, usage, and the purpose of the repository. It’s ready for your GitHub!
