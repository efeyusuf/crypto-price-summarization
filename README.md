# Code and Data Files Overview

This repository contains various code and data files used in the project. Below is a detailed explanation of each file:

## Code Files

- **Training_Data_Generation**: 
  - Description: Utilizes OpenAI's API to generate a synthetic dataset. This dataset includes arbitrary price changes, corresponding sets of 10 tweets, and a summary for each set.
  
- **train_data_eval**: 
  - Description: Evaluates the consistency between the given price changes & tweets and the resulting summary. Essential for ensuring the quality of the training data, given that labels were not human-generated.
  
- **Tweet_Clustering**: 
  - Description: Classifies tweets into different groups for inference purposes.

- **Llama2_finetune**: 
  - Description: Employs Huggingface's AutoTrain module to finetune the Llama2-7b model using techniques like quantization and low-rank adaptation.

- **Llama-inference_yusufefe**: 
  - Description: Used for testing the outputs of the finetuned model.

## Data Files

- **train_data**: 
  - Description: The synthetic dataset generated using the Training_Data_Generation script.

- **twitter-data-bitcoin**: 
  - Description: A real-world dataset about Bitcoin, scraped with specific filters (English language, over 10k followers).

## Additional Notes

- The synthetic dataset and evaluation steps are crucial for training robust models as they provide a controlled environment to test and improve the model's performance.
- The real-world Bitcoin dataset adds practical relevance and helps in fine-tuning the model to understand and interpret real-world data effectively.


