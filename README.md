# Overview

All data processing and model training was done in jupyter notebook using python. Datasets are stored in the form of .csv files

# Models

The models were trained in "BinaryFullyTrained.ipynb" using pytorch and huggingface's transformer library. 
The "BinaryFewShot.ipynb" and "MutliClassification.ipynb" notebooks were used to train other versions of the model which were utlimately not used or discussed in the final paper. 
"GPT.ipynb" was used for comparison with GPT-3.5 using zero-shot and few-shot learning. 

# Datasets

"bragging_data.csv" contains the original bragging data used for initial training, this model was originally made by Jin et al. (https://aclanthology.org/2022.acl-long.273.pdf)

The first 10000 lines of the 2022 Russell 1000 firm transcripts are available in "transcript_first-2022.csv" 

Because quotes were seperated across multiple columns, "transcript_combined.csv" combines all text from each speaker into one column

Subsequently, "transcript_combined2.csv" removes all words from "Operator" 

Finally, "transcript_final.csv" filters for only text from the company spokesperson. 

# Results

Responses from GPT - 3.5 (zero shot) are stored in "GPT3zeroshotGuess.csv" 

Responses from GPT - 3.5 (few shot) are stored in "GPT3fewshotGuess.csv" 

Final bragging scores for transcripts are stored in "scores.csv" 

