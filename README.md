# Questioning

# Project Overview

This project evaluates large language models (LLMs) on their ability to generate curiosity-driven questions. Utilizing a unique framework called CDQG (Curiosity-Driven Question Generation), we explore the performance of eight different LLMs, focusing on how they formulate questions based on given statements.

## Directory Structure

- **Combined_files/**: Consolidated outputs for easy reference.
- **Dataset/**: Initial prompts categorized by subject (Physics, Chemistry, Math) and difficulty level, serving as input for the LLMs.
- **Final_combined_CSV_files/**: Aggregated results featuring model outputs alongside generated questions.
- **Instruction_questions_all_models/**: Direct model outputs based on specific instructions.
- **Outputs_{model_name}/**: Individual outputs from each of the eight models.
- **Human Evaluation Files/**: Contains the final evaluations where the Gemini model has synthesized the outputs from GPT-4, Mistral, and itself into final scores for relevance, coherence, and diversity.
- **.ipynb files**: Jupyter notebooks for data processing and analysis.
- **README.md**: This document.

## Environment Setup

Ensure Python and necessary libraries (Pandas, Numpy, shutil) are installed:

## Execution Instructions

1. **Repository Setup**: Clone the repository and navigate to the project directory.
2. **Data Analysis**: Launch Jupyter to access notebooks:


## Data Description

Each CSV file within the folders is named systematically to reflect its contents, which include:
- Model name
- Metric evaluated (Relevance, Coherence, Diversity)
- Data type (e.g., basic, intermediate, advanced)

## Model Details

The project utilizes eight LLMs for question generation. Three of these models (GPT-4, Gemini, Mistral) are further used to evaluate the generated questions. Gemini synthesizes these evaluations to produce a final assessment captured in the `Human Evaluation Files`.

## Results and Discussion

The findings from this project highlight the capabilities and limitations of current LLMs in generating diverse and relevant questions. These results are pivotal for guiding future developments in AI-driven questioning and educational tools.

## Contributions and Collaboration

We encourage contributions that enhance model evaluations or extend dataset utility. Please see our contributing guidelines linked in this repository.

## Contact Information

For inquiries or further information, please contact [Your Contact Information].
