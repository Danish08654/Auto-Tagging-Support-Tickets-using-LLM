#  Auto Tagging Support Tickets using LLM

This project focuses on automatically tagging customer support tickets into relevant categories using a Large Language Model (LLM).

The system leverages prompt engineering, few-shot learning, and fine-tuning techniques to classify free-text support tickets and output the **top 3 most probable tags**.



##  Objective

- Automatically classify support tickets into categories  
- Compare:
  - Zero-shot learning
  - Few-shot learning
  - Fine-tuned model performance  
- Improve tagging accuracy using LLM techniques  
- Output **Top-3 predicted tags** for each ticket  


##  Dataset

The dataset contains real-world styled support tickets with fields such as:

- Ticket Subject  
- Ticket Description  
- Ticket Type (label)  
- Priority, Channel, Resolution, etc.  

 Only **text fields** (subject + description) are used for tagging.


##  Methodology

###  1. Data Preprocessing
- Combined text fields:

-  Cleaned and formatted input text


###  2. Zero-Shot Learning

- Used LLM without training  
- Prompt-based classification  

###  3. Few-Shot Learning

- Added examples in prompt  
- Improved contextual understanding  


###  4. Fine-Tuning (Optional Advanced Step)

- Trained model on labeled dataset  
- Used transformer-based model (e.g., BERT / FLAN-T5)  
- Evaluated performance improvement  


###  5. Top-3 Tag Prediction

Instead of single label, model predicts:

1. Billing
   
2. Technical Issue
   
3. Product Inquiry
