This project is a part of the HKU-DASC7606 course.

The eval_fewshot.py is the main script in this project.

model and embedder can be downloaded by running download.py 
	model: Phi-1_5 https://huggingface.co/microsoft/phi-1_5 or Phi-2 https://huggingface.co/microsoft/phi-2
	embedder: bge-small-en-v1.5 https://huggingface.co/BAAI/bge-small-en-v1.5

For Hyperparameter tuning, four key parameters in Phi models: 
	N: number of examples in one prompt; 
	Max_len: the maximum length allowed for the input; 
	Top_k: Boolean variable controlling selections of similar examples for in-context learning; 
	Top_k_reverse: Boolean variable controlling the order of similar examples when appending. 

To reproduce the final result in the report, please use the following command:

CALL conda activate nlp_env
CALL cd /d your_path
CALL python acc.py --prediction_path model_predictions/Easy
CALL python acc.py --prediction_path model_predictions/Challenge

Please contact yl9919@connect.hku.hk for any inquiries. 
