# Midjourney Prompt Clustering

Processing and clustering Midjourney prompts using NLP techniques to identify potential use cases for text-to-image generation models.

This repo stems from my data mining project for the CU Boulder MSDS [DTSA 5506 course](https://www.coursera.org/specializations/data-mining-foundations-practice).

Course Instructor: Dr. Qin (Christine) Lv, Associate Professor of Computer Science.

## Project Description

This project addresses the scope for refinement in text-to-image diffusion models with a case study of Midjourney. The analysis utilizes a large dataset of 55,082,563 Midjourney prompts used between April 8th and August 25th, 2023 [1]. The primary objective is to use data mining techniques to identify potential application areas for these generative models, using natural language processing (NLP) and k-means clustering.

Key goals include:
- Engineering salient features from prompt text strings
- Applying k-means clustering to identify associated groups of prompts  
- Inferring potential use cases and application areas from the resulting clusters

This builds on prior work examining characteristics of image generation prompts [2][3] and aims to contribute insights for optimizing text-to-image models.

## Methodology

The approach involves:
1. Exploratory data analysis on a sample of 1 million prompts
2. Feature engineering using NLP techniques like term frequency and entity extraction
3. Vectorization of prompts using TF-IDF 
4. K-means clustering to identify associated groups of prompts
5. Qualitative analysis of resulting clusters to infer use cases

## Key Findings

Several promising clusters were identified, suggesting potential specialized use cases:

- Scene generation featuring specific characters
- Detailed artistic photography  
- Coloring book style illustrations
- Image transformation and blending
- Children's cartoon generation
- Logo creation with text elements
- Graphics on white backgrounds

These point to broader categories like entertainment and graphic design, as well as more specific applications like photography environment emulation.

## Dataset

The prompt dataset for this project is available on HuggingFace thanks to Ming Yang: 
[vivym/midjourney-messages](https://huggingface.co/datasets/vivym/midjourney-messages) [1].

## Setup

The `data-mining.ipynb` notebook is the main entrypoint for this project/repo. Each step of the process is documented with code snippets and commentary.

1. Clone the repository.
2. Download and place the required parquet files in the `data/` directory.
3. Open the `data-mining.ipynb` notebook to review and run the implemented algorithms.

### Files

- `data/`: This directory should contain the source parquet files.  
- `data-mining.ipynb`: Primary Jupyter notebook containing analysis.

## Challenges and Limitations

Key challenges encountered include:
- Lack of strong quantitative evaluation metrics for clustering results
- Computational intensity of processing large text datasets
- Limitations of the chosen NLP and clustering techniques

Future work could explore more advanced NLP methods like word embeddings, as well as techniques for programmatically labeling resulting clusters.

## References

[1] Yang, M. (2023). vivym/midjourney-messages. Dataset. HuggingFace. https://huggingface.co/datasets/vivym/midjourney-messages

[2] Liao, S., & Ji, X. (2023). A Study on the Application of Generative Artificial Intelligence Technology in Image Design. https://doi.org/10.2991/978-94-6463-266-8_36

[3] Wang, Z. J., Montoya, E., Munechika, D., Yang, H., Hoover, B., & Chau, D. H. (2023). DiffusionDB: A Large-scale Prompt Gallery Dataset for Text-to-Image Generative Models. ArXiv:2210.14896 [cs.CV]. https://arxiv.org/abs/2210.14896

## Contributions

Feel free to fork the project and make your contributions. Should you find discrepancies, or wish to suggest improvements, please open an issue or submit a pull request.

The content of this repository is licensed under a [MIT License](https://choosealicense.com/licenses/mit/).
