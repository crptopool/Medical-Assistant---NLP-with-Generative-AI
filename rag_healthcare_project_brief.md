# RAG-Based AI Solution for Healthcare Decision Support

## Business Context

The healthcare industry is rapidly evolving, and professionals face increasing challenges in managing vast volumes of medical data while delivering accurate and timely diagnoses. Quick access to comprehensive, reliable, and up-to-date medical knowledge is critical for improving patient outcomes and ensuring informed decision-making in a fast-paced environment.

Healthcare professionals often encounter information overload, struggling to sift through extensive research and data to create accurate diagnoses and treatment plans. This challenge is amplified by the need for efficiency, particularly in emergencies, where time-sensitive decisions are vital. Furthermore, access to trusted, current medical information from renowned manuals and research papers is essential for maintaining high standards of care.

To address these challenges, healthcare centers can focus on integrating systems that streamline access to medical knowledge, provide tools to support quick decision-making, and enhance efficiency. Leveraging centralized knowledge platforms and ensuring healthcare providers have continuous access to reliable resources can significantly improve patient care and operational effectiveness.

---

## Objective

As an AI specialist, your task is to develop a **RAG-based AI solution** using renowned medical manuals to address healthcare challenges.

The objective is to:

- Understand information overload in healthcare.
- Apply AI techniques to streamline decision-making.
- Analyze the impact of AI-assisted search and retrieval on diagnostics and patient outcomes.
- Evaluate the potential of RAG systems to standardize care practices.
- Create a functional prototype demonstrating feasibility and effectiveness.

---

## Questions to Answer

The solution should answer the following medical questions:

1. **Sepsis Management**  
   What is the protocol for managing sepsis in a critical care unit?

2. **Appendicitis**  
   What are the common symptoms of appendicitis, and can it be cured via medicine?  
   If not, what surgical procedure should be followed to treat it?

3. **Sudden Patchy Hair Loss**  
   What are the effective treatments or solutions for addressing sudden patchy hair loss, commonly seen as localized bald spots on the scalp?  
   What could be the possible causes behind it?

4. **Brain Tissue Injury**  
   What treatments are recommended for a person who has sustained a physical injury to brain tissue, resulting in temporary or permanent impairment of brain function?

5. **Leg Fracture During Hiking**  
   What are the necessary precautions and treatment steps for a person who has fractured their leg during a hiking trip?  
   What should be considered for their care and recovery?

---

## Data Dictionary

### Merck Manuals

The **Merck Manuals** are medical references published by the American pharmaceutical company **Merck & Co.** They cover a wide range of medical topics, including:

- Disorders
- Tests
- Diagnoses
- Drugs
- Treatment approaches
- Clinical guidance

The manuals have been published since **1899**, when Merck & Co. was still a subsidiary of the German company Merck.

The provided manual is a PDF with over **4,000 pages**, divided into **23 sections**.

---

## Important Runtime Note

Please set the runtime to **T4-GPU** in Google Colab.

### Steps to Set Runtime to GPU in Google Colab

1. Click on **Runtime** in the menu bar.
2. Select **Change runtime type** from the dropdown menu.
3. In the **Hardware accelerator** section, choose **GPU**.
4. If multiple GPU options are shown, choose **GPU** if you specifically want a T4 GPU.
5. Click **Save**.

---

# Submission Guidelines

There are two ways to work on this project:

1. **Full-code way**
2. **Low-code way**

The primary purpose of providing these two options is to allow learners to choose the approach that aligns with their learning aspirations and career outcomes.

---

## Submission Options

| Submission Type | Who Should Choose | What Is the Same Across Both | What Is Different | Final Submission File | Submission Format |
|---|---|---|---|---|---|
| **Full-code** | Learners who aspire to be in hands-on coding roles and want to build solution code from scratch | Perform exploratory data analysis to identify insights and recommendations for the problem | Focus on code writing. Around 10–20% grading may be based on the quality of the final code submitted | Solution Python notebook from the full-code template submitted in HTML format | `.html` |
| **Low-code** | Learners who aspire to be in managerial roles and want to focus on solution review, interpretation, recommendations, and business communication | Perform exploratory data analysis to identify insights and recommendations for the problem | Focus on business presentation. Around 10–20% grading may be based on the quality of the final presentation submitted | Business presentation with problem definition, insights, and recommendations | `.pdf` |

---

## General Submission Instructions

Please follow the steps below to complete the assessment.

> **Important:** If you submit a presentation, **only the presentation will be evaluated**. Make sure that all sections mentioned in the rubric are covered in your submission.

---

## Full-Code Version

1. Download the full-code version of the learner notebook.
2. Follow the instructions provided in the notebook to complete the project.
3. Write down insights and recommendations for the business problems in the comments.
4. Submit only the solution notebook prepared from the learner notebook.

### Required Format

- Submit as: `.html`
- Do **not** submit as: `.ipynb`

---

## Low-Code Version

1. Download the low-code version of the learner notebook.
2. Follow the instructions provided in the notebook to complete the project.
3. Prepare a business presentation with insights and recommendations for the business problem.
4. Submit only the presentation.

### Required Format

- Submit as: `.pdf`
- Do **not** submit as: `.pptx`

---

## Important Submission Rules

1. Any assignment found copied or plagiarized from other submissions will not be graded and will be awarded **zero marks**.
2. Please ensure timely submission. Any submission after the deadline will not be accepted for evaluation.
3. Submission will not be evaluated if:
   - It is submitted after the deadline.
   - More than one file is submitted.

---

# Best Practices for Full-Code Submissions

The final Python notebook should be:

- Well-documented.
- Supported with inline comments explaining the functionality of the code.
- Supported with markdown cells containing observations and insights.
- Run sequentially from start to finish before submission.
- Free from warnings and errors.

### Important

- Submit the notebook as an **HTML file**.
- Do **not** submit the notebook as an `.ipynb` file.
- Refer to the FAQ page for common project-related queries.

---

# Best Practices for Low-Code Submissions

The presentation should be prepared with the assumption that the audience is the **Data Science Lead of a company**.

## Key Points to Include

The presentation should include:

- Business overview of the problem.
- Solution approach.
- Key findings and insights that can drive business decisions.
- Business recommendations.
- Key takeaways explained in an easy-to-understand manner.
- Potential benefits of implementing the solution.

## Important Presentation Guidance

- Avoid copying and pasting directly from the notebook.
- Avoid showing code unless code is the focal point of the presentation.
- Submit the presentation as a **PDF file**.
- Do **not** submit the presentation as a `.pptx` file.
- Refer to the FAQ page for common project-related queries.

---

# Power Ahead!

---

# Rubric

## Rubric Summary

| Criteria | Requirements | Points |
|---|---|---:|
| **Question Answering using LLM** | Load the large language model from Hugging Face; create a function to define model parameters and generate a response; apply the response generation function to answer the questions; provide comments and observations for the answers received | 8 |
| **Question Answering using LLM with Prompt Engineering** | Apply prompt engineering and LLM parameter tuning using at least 5 combinations; answer the questions provided in the problem statement; provide comments and observations for the answers received | 11 |
| **Data Preparation for RAG** | Load the data file; split the data using a text splitter with necessary attributes; load the embedding model; load the vector database; define the retriever with appropriate search method and `k` value | 8 |
| **Question Answering using RAG** | Get answers to the questions; fine-tune chunking, retriever, and LLM parameters using at least 5 combinations; provide comments and observations for the answers received | 12 |
| **Output Evaluation** | Define the evaluation prompt for groundedness; define the evaluation prompt for relevance; evaluate all responses for the questions provided in the problem statement | 9 |
| **Actionable Insights and Recommendations** | Provide key takeaways for the business | 4 |
| **Presentation / Notebook - Overall Quality** | Structure and flow; crispness; visual appeal; conclusion and business recommendations; or, for notebook submission, structure and flow, well-commented code, conclusion, and business recommendations | 8 |

---

## Total Points

**60 points**

---

# Suggested Final Deliverables Checklist

## For Full-Code Submission

- [ ] Notebook runs end-to-end without errors.
- [ ] Large language model loaded from Hugging Face.
- [ ] Response generation function created.
- [ ] All five medical questions answered using base LLM.
- [ ] At least five prompt engineering / parameter tuning combinations tested.
- [ ] Medical manual PDF loaded.
- [ ] Text split into chunks.
- [ ] Embedding model loaded.
- [ ] Vector database created.
- [ ] Retriever configured with search method and `k` value.
- [ ] RAG responses generated for all five questions.
- [ ] At least five RAG tuning combinations tested.
- [ ] Groundedness evaluation prompt defined.
- [ ] Relevance evaluation prompt defined.
- [ ] All responses evaluated.
- [ ] Business insights and recommendations included.
- [ ] Notebook exported as `.html`.

## For Low-Code Submission

- [ ] Problem definition included.
- [ ] Business context explained.
- [ ] Solution approach explained.
- [ ] RAG workflow described.
- [ ] Key findings included.
- [ ] Answers to all five medical questions summarized.
- [ ] Groundedness and relevance evaluation explained.
- [ ] Business recommendations included.
- [ ] Benefits of implementation included.
- [ ] Presentation exported as `.pdf`.

---

# Notes

This project focuses on demonstrating how Retrieval-Augmented Generation can help healthcare professionals access trusted medical knowledge quickly and consistently.

The solution should emphasize:

- Accuracy
- Groundedness
- Relevance
- Explainability
- Speed of access to medical knowledge
- Standardization of care practices
- Potential impact on patient outcomes
