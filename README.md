# Financial LLM Fine-Tuning on AWS

This project demonstrates how to fine-tune the Meta Llama 2 7B large language model for financial domain expertise using AWS SageMaker.

## Overview

This project aims to improve the domain-specific knowledge and generation capabilities of the Meta Llama 2 7B model by fine-tuning it on a financial dataset. The process involves evaluating the base model on financial prompts, fine-tuning it using AWS SageMaker, and then comparing its performance to the base model.

## Key Steps

1. **Model Evaluation**: Test the base Llama 2 7B model on financial prompts.
2. **Fine-Tuning**: Fine-tune the model on a financial dataset using AWS SageMaker.
3. **Evaluation**: Compare the fine-tuned model's performance to the base model.

## Files

- **Model_Evaluation_UdacityGenAIAWS.ipynb**: Notebook for evaluating the base Llama 2 7B model.
- **Model_FineTuning.ipynb**: Notebook for fine-tuning the model and evaluating the results.
- **financialDataset.txt**: Dataset used for fine-tuning (stored in S3).

## Setup

### Step 1: Upload Project Starter Files

1. Start your SageMaker Notebook Instance by clicking on **Open JupyterLab** once your notebook instance is ready.
   ![AmzSagemakerModels](https://github.com/user-attachments/assets/ff849672-39a9-415e-af57-a49c681e4b9b)

2. Upload the 2 Python notebook files (.ipynb) in the project starter files folder to JupyterLab using the upload arrow in the top left menu.
   ![AmzS3DataBucket](https://github.com/user-attachments/assets/f613fd6e-5ba0-47ba-ace0-d5b094ebd314)


3. You should see two Jupyter Notebook files in the JupyterLab file menu. Use the **Python 3.10 PyTorch or TensorFlow Kernel** to run code in these notebooks.

4. Remember to stop your notebook instance when you stop or pause work on your project. Save your individual notebook files periodically in JupyterLab using the **File -> Save** menu to avoid losing your work between sessions.
   ![screen-shot-2024-01-07-at-1 53 29-pm](https://github.com/user-attachments/assets/119381fa-8011-48f7-b19c-4d593ece887b)


### Step 2: Choose Your Dataset

1. In the project notebook files, select the domain for your model:
   - Financial domain
   - IT domain
   - Healthcare/Medical domain

2. Fill out the domain you've selected in the Project Documentation Report.

### Step 3: Deploy and Evaluate the Model

1. Complete and run the cells in the `Model_Evaluation.ipynb` file.
2.  Save and download your `Model_Evaluation.ipynb` with the cell output.
3. Ensure you've run the cells that delete the model deployment and endpoint to avoid unnecessary charges.

### Step 4: Fine-Tune the Model

1. Complete and run the cells in the `Model_FineTuning.ipynb` file.
2. Download your `Model_FineTuning.ipynb` with the cell output.

### Step 5: Deploy and Evaluate the Fine-Tuned Model

1. Visit the AWS S3 bucket where your fine-tuned model weights are stored after training.
2. Complete and run the cells in the `Model_FineTuning.ipynb` file about deploying and evaluating the fine-tuned model.
3. Ensure you've run the cells that delete the model deployment and endpoint to avoid unnecessary charges.



## Results

The fine-tuned model shows improved performance on financial prompts, demonstrating more domain-specific knowledge and relevant content generation compared to the base model.

## Caution

Remember to delete your SageMaker endpoints after use to avoid unnecessary charges.

---

By fine-tuning the Meta Llama 2 7B model on a financial dataset, this project highlights the potential for large language models to adapt and excel in specific domains, providing more accurate and relevant outputs for financial applications.
