
#Automatic Language Detection (WiLI-2018)  

#Project Overview  
This project compares three machine learning and deep learning approaches for **automatic language detection** using a subset of the **WiLI-2018 dataset**.  

The models compared are:  
- TF-IDF + Logistic Regression** (classical ML baseline)  
- LSTM with Character Embeddings** (deep learning approach)  
- XLM-RoBERTa** (Transformer-based pretrained model, fine-tuned for language detection)  
---

 #Dataset  
- Source:** [WiLI-2018 Wikipedia Language Identification dataset](https://zenodo.org/record/841984)  
- Total languages available: 235  
- Languages used in this project:** 10 (restricted for faster training and comparison)  
---
# Models Implemented  
1. **TF-IDF + Logistic Regression**  
- Text → TF-IDF vectors (char n-grams)  
- Logistic Regression for classification
  
2. **LSTM**  
- Character-level tokenization  
- LSTM network learns sequential patterns  
- Dense output layer for classification  

3. **Transformer (XLM-RoBERTa)**  
- Pretrained `xlm-roberta-base` model  
- Input: `input_ids` + `attention_mask`  
- Fine-tuned on labeled dataset  


