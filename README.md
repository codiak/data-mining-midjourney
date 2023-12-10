# Midjourney Prompt Clustering (DTSA 5506 Data Mining Project)

Processing and clustering Midjourney prompts using NLP techniques.

This repo stems from my data mining project for the CU Boulder MSDS [DTSA 5506 course](https://www.coursera.org/specializations/data-mining-foundations-practice).

Course Instructor: Dr. Qin (Christine) Lv, Associate Professor of Computer Science.

## Project Description

This project addresses the scope for refinement in text-to-image diffusion models with the case study of Midjourney. The analysis utilizes a large dataset of 55,082,563 Midjourney prompts used between April 8th and August 25th, 2023. The primary objective is to use data mining techniques to identify potential application areas for these generative models, using natural language processing (NLP) and k-means clustering.

## Dataset

The prompt dataset for this project can be obtained from: [vivym/midjourney-messages](https://huggingface.co/datasets/vivym/midjourney-messages).

## Setup

The `data-mining.ipynb` notebook is the main entrypoint for this project/repo. Each step of the process is documented with code snippets and commentary.

1. Clone the repository.
2. Download and place the required parquet files in the `data/` directory.
3. Open the `data-mining.ipynb` notebook to review and run the implemented algorithms.

### Files

- `data/`: This directory should contain the source parquet files.
- `data-mining.ipynb`: Primary Jupyter notebook.

## Contributions

Feel free to fork the project and make your contributions. Should you find discrepancies, or wish to suggest improvements, please open an issue or submit a pull request.

The content of this repository is licensed under a [MIT License](https://choosealicense.com/licenses/mit/).
