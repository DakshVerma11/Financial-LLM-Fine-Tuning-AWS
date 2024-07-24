Financial LLM Fine-Tuning on AWS
This project demonstrates how to fine-tune the Meta Llama 2 7B large language model for financial domain expertise using AWS SageMaker.

Overview
We evaluate the base Llama 2 7B model on financial prompts, then fine-tune it on a financial dataset to improve its domain-specific knowledge and generation capabilities.
Key Steps

Model Evaluation: Test the base Llama 2 7B model on financial prompts
Fine-Tuning: Fine-tune the model on a financial dataset using AWS SageMaker
Evaluation: Compare the fine-tuned model's performance to the base model

Files

Model_Evaluation_UdacityGenAIAWS.ipynb: Notebook for evaluating the base Llama 2 7B model
Model_FineTuning.ipynb: Notebook for fine-tuning the model and evaluating the results
financialDataset.txt: Dataset used for fine-tuning (stored in S3)

Setup

Ensure you have the necessary AWS permissions and SageMaker setup
Upload the financialDataset.txt to your S3 bucket
Update the S3 path in Model_FineTuning.py to point to your dataset

Usage

Run Model_Evaluation_UdacityGenAIAWS.py to evaluate the base model
Run Model_FineTuning.py to fine-tune the model and evaluate the results
Compare the outputs to see the improvement in financial domain knowledge

Results
The fine-tuned model shows improved performance on financial prompts, demonstrating more domain-specific knowledge and relevant content generation compared to the base model.


Caution
Remember to delete your SageMaker endpoints after use to avoid unnecessary charges.

