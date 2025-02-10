# 🤔 Questioning

# 🎯 Project Overview

This project evaluates large language models (LLMs) on their ability to generate curiosity-driven questions. Utilizing a unique framework called CDQG (Curiosity-Driven Question Generation), we explore the performance of eight different LLMs, focusing on how they formulate questions based on given statements.

## 📂 Directory Structure

<div style="background-color: #f8f9fa; padding: 15px; border-radius: 5px;">

- **📁 Combined_files/**: Consolidated outputs for easy reference. It contains the Instruction, the output given by certain model and the evaluation done by Mistral, Gemini and GPT.
- **📊 Dataset/**: Initial statements categorized by subject (Physics, Chemistry, Math) and difficulty level, serving as input for the LLMs.
- **📈 Final_combined_CSV_files/**: Aggregated results featuring model outputs alongside generated questions.
- **📝 Instruction_questions_all_models/**: Direct model outputs based on specific instructions.
- **🤖 Outputs_{model_name}/**: Individual outputs from each of the eight models for the statements, which is basically the quesitons created by the model for each of the statement.
- **👥 Human Evaluation Files/**: Contains the final evaluations where the Gemini model has synthesized the outputs from GPT-4, Mistral, and itself into final scores for relevance, coherence, and diversity and also the corresponding Human Evaluated results.
- **📓 .ipynb files**: Jupyter notebooks for data processing and analysis.
- **📊 Final Eval**: Contians all final evaluations where the Gemini model has synthesized the outputs from GPT-4, Mistral, and itself into final scores for relevance, coherence, and diversity
- **📖 README.md**: This document.
</div>

## ⚙️ Environment Setup

<div style="background-color: #e6f3ff; padding: 15px; border-radius: 5px;">

Ensure Python and necessary libraries (Pandas, Numpy, shutil, transformers, accelerate, torch, tqdm) are installed:
</div>

## 🚀 Execution Instructions

<div style="background-color: #f0fff4; padding: 15px; border-radius: 5px;">

1. **Repository Setup**: Clone the repository and navigate to the project directory.
2. **Data Analysis**: Launch Jupyter to access notebooks:
</div>

## 📊 Data Description

<div style="background-color: #fff5f5; padding: 15px; border-radius: 5px;">

Each CSV file within the folders is named systematically to reflect its contents, which include:
- Model name
- Metric evaluated (Relevance, Coherence, Diversity)
- Data type (e.g., basic, intermediate, advanced)
</div>

## 🤖 Model Details

<div style="background-color: #f0f0ff; padding: 15px; border-radius: 5px;">

The project utilizes eight LLMs for question generation. Three of these models (GPT-4, Gemini, Mistral) are further used to evaluate the generated questions. Gemini synthesizes these evaluations to produce a final assessment captured in the `Human Evaluation Files`.
</div>

## 📈 Results and Discussion

<div style="background-color: #fffff0; padding: 15px; border-radius: 5px;">

The findings from this project highlight the capabilities and limitations of current LLMs in generating diverse and relevant questions. These results are pivotal for guiding future developments in AI-driven questioning and educational tools.
</div>

## 🤝 Contributions and Collaboration

<div style="background-color: #f8f4ff; padding: 15px; border-radius: 5px;">

We encourage contributions that enhance model evaluations or extend dataset utility. Please see our contributing guidelines linked in this repository.
</div>

# 🧪 Chemistry Learning Analysis Example

## 📝 Initial Statement
> **"Organic chemistry focuses on compounds containing carbon."**

## 🎯 Prompt

> Imagine you are a human, this is the first time you are coming across this Chemistry Statement, you have no previous knowledge of it <b>"Organic chemistry focuses on compounds containing carbon."</b>, what are the top 5 questions that would pop up in your head which would be most useful in learning about it as you are new to it. Give me a simple bullet point list, don't explain them or expand them.

## 📊 Detailed Evaluation Results

| Instruction | Model Output | <span style="color: #9932CC">Mistral Output</span> | <span style="color: #4169E1">Gemini Output</span> | <span style="color: #228B22">GPT Output</span> |
|-------------|--------------|----------------|---------------|------------|
| Imagine you are a human... | • What exactly is carbon, and why is it so important in organic chemistry?<br><br>• How do organic compounds differ from inorganic compounds, and what are some common types of organic compounds?<br><br>• What is the difference between saturated and unsaturated hydrocarbons, and how do they behave differently in chemical reactions?<br><br>• How do functional groups affect the properties and behavior of organic compounds? | <span style="color: #9932CC">Coherence: 4/5<br>Relevance: 5/5<br>Diversity: 4/5<br><br>*Questions follow logical progression, moving from basic concepts to more specific topics.*</span> | <span style="color: #4169E1">Relevance: 4/5<br>Coherence: 4/5<br>Diversity: 3/5<br><br>*Questions directly related to statement, form coherent line of inquiry.*</span> | <span style="color: #228B22">Relevance: 5/5<br>Coherence: 4/5<br>Diversity: 5/5<br><br>*Questions directly pertain to concepts, logical progression.*</span> |

### 🎯 Final Gemini Evaluation
<div style="background-color: #e6f3ff; padding: 10px; border-radius: 5px;">

| Metric | Average Score | Description |
|--------|---------------|-------------|
| 🎯 Relevance | <span style="color: #008000">4.5/5</span> | Questions strongly aligned with core concept |
| 🔄 Coherence | <span style="color: #0000FF">4.0/5</span> | Good logical flow from basic to advanced concepts |
| 🌈 Diversity | <span style="color: #800080">4.0/5</span> | Balanced coverage of different aspects |
</div>

### 👤 Human Validation Scores
<div style="background-color: #fff5e6; padding: 10px; border-radius: 5px;">

- 🎯 Relevance: <span style="color: #FF4500">3.0/5</span>
- 🔄 Coherence: <span style="color: #FF4500">3.0/5</span>
- 🌈 Diversity: <span style="color: #FF4500">3.0/5</span>
</div>

## Contact Information

For inquiries or further information, please contact shashi ( sjavaji@stevens.edu ).
