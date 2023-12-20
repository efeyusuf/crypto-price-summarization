Here are the code/data files and their explanations:

Training_Data_Generation: Used OpenAI's API to generate a data set, which outputs an arbitrary price change, corresponding 10 tweets, and a final summary
train_data: Resulting synthetic data set
train_data_eval: Checked the consistency scores between the given price changes & tweets and the resulting summary. Since the labels were not human-generated, this step was needed to ensure the quality of the training data.
twitter-data-bitcoin: It is the real-world dataset about Bitcoin, which I scraped (some filters I applied in my scraping: (English, over 10k followers)
Tweet_Clustering: Used to classify tweets into groups for inference purposes. 
Llama2_finetune: Used huggingface's autotrain module to finetune the Llama2-7b model by quantization and low-rank adaptation.
Llama-inference_yusufefe: Used for testing model outputs

