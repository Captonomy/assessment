# Machine Learning Engineer Assignment: Document Classification and Information Extraction

Dear Candidate,

Thank you for your interest in the Machine Learning Engineer position at Captonomy Consulting. To assess your understanding of Transformer Models and practical machine learning skills, we have prepared an assignment that mirrors some of the challenges you might encounter in our R&D team.

## Assignment Overview

You will be provided with a folder containing PDF files. Each PDF is the first page of a paper submitted to ICDAR 2024 (International Conference on Document Analysis and Recognition). Your tasks are:

1. **Information Extraction**: Extract the **title** and **authors** from each paper.
2. **Document Classification**: Classify each paper into one of the predefined categories (or suggest better-fitting ones if applicable).
3. **Organize Outputs**: Create a json file with the classification and extraction results.

### Our Predefined Categories

- **Tables**
- **Classification**
- **Key Information Extraction**
- **Optical Character Recognition**
- **Datasets**
- **Document Layout Understanding**
- **Others**

*Feel free to suggest and use other categories if you believe they fit better (either extra ones or even totally new set of classes). A maximum of 10 categories are acceptable.*

## Technical Requirements

The resulting code should be able to **run offline on a local machine**. If a GPU is required you can use Google Collab or similar service for your development.

- **Model Usage**: You are free to utilize any open source algorithm of your choosing (from classical ML scikit ones to Deep Learning models) and are encouraged to prefer small models like **BERT-like encoders** or similar. You may use pre-trained versions and fine-tune them if necessary.
- **Programming Language**: Python is mandatory.
- **Libraries and Tools**: You are encouraged to use libraries such as PyTorch (preferred), TensorFlow, Hugging Face Transformers, or any other relevant tools.

## Detailed Instructions

### 1. Information Extraction

- **Objective**: Extract the **title** and **authors** from each PDF and save them in json format.

### 2. Document Classification

- **Objective**: Classify each paper into the most appropriate category.
- **Guidelines**:
    - Analyze the content (title, abstract, etc.) to determine the relevant category.
    - Use BERT-like models to generate embeddings or for text classification.
    - If you believe a paper doesn't fit any of the predefined categories, you may classify it under **"Others"** or propose a new category.

### 3. Output

- **Objective**: Create a JSON file with your output, based on the following schema.

```
{
  "tables": [{"originalFileName": "paper_A.pdf", "title": "recognized title", "authors": ["author_A", "author_B"]},
            {"originalFileName": "paper_B.pdf", "title": "recognized title", "authors": ["author_C", "author_D"]},
            ...],
  "classification": [...],
  "keyInformationExtraction": [...],
  "opticalCharacterRecognition": [...],
  "datasets": [...],
  "layoutUnderstanding": [...],
  "others": [...]
}
```
- **Guidelines**:
    - You can optionally use the provided CSV to do a sanity check and validate your results.

## Deliverables

1. **Code**:
    - Provide all scripts and code used to complete the assignment. Jupyter Notebook format is preferred.
    - Your code should be well-documented and organized.
    - Include a `README.md` file with instructions on how to configure and run your code.
    - Include a `requirements.txt` file if necessary.

2. **Results**:
    - Include the generated json file from your own inference run.

3. **Report**:
    - A brief report (max 2 pages) that could include (but not mandatory):
        - **Introduction**: Overview of your approach.
        - **Methodology**: Explanation of the models and techniques used for information extraction and classification.
        - **Challenges**: Any issues faced during the assignment and how you addressed them.
        - **Conclusion**: Summary of your findings and any suggestions for improvement.

## Evaluation Criteria

- **Accuracy of Information Extraction**: Correctness in extracting titles and authors.
- **Classification Performance**: Proper category assignment.
- **Use of Machine Learning Models**: Effective utilization of classical and/or deep learning models in your solution.
- **Code Quality**: Readability, organization, and documentation of your code.
- **Problem-Solving Skills**: Methodology used to tackle the underlying issue.
- **Communication**: Clarity and conciseness of your report.

## Submission Guidelines

- **Time Spent**: You are free to spend as much time as necessary. However, we expect the task to not take more than a few workdays.
- **Submission**: Send your archive via email to [Insert Email Address], or provide a link to a GitHub repository if you prefer.
- **Naming Convention**: Name your archive `YourName_MLE_Assignment.zip`.

## Additional Information

- **Data Privacy**: Ensure that any code or data shared complies with data privacy laws and regulations.
- **Assumptions**: Clearly state any assumptions you make during the assignment.
- **Questions**: If you have any questions or need clarifications, feel free to reach out to us at [Insert Contact Information].

---

We look forward to seeing your innovative solutions and insights!

Best regards,

The Captonomy Consulting Team
