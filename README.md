# **Urdu-to-English Machine Translation using LSTM with Attention**  

## **Overview**  
This project implements an **LSTM-based attention encoder-decoder model** for **machine translation from Urdu to English** using **PyTorch**. The model is trained on a **parallel dataset** and evaluated using **BLEU scores** to measure translation quality.  

## **Dataset**  
- **Source**: Provided parallel dataset (sentence-aligned).  
- **Preprocessing**:  
  - Merge `.dev` and `.devtest` files.  
  - Shuffle and split into **70% training**, **15% validation**, and **15% test**.  

## **Model Architecture**  
- **Encoder**: Bi-directional **LSTM** processes Urdu input sequences.  
- **Attention Mechanism**: Enhances focus on relevant words during decoding.  
- **Decoder**: LSTM generates translated English text based on encoder outputs and attention.  
- **Implementation**: Custom PyTorch model (no pre-built RNN libraries used).  

## **Evaluation**  
- **Train & Validation Metrics**:  
  - Loss curve visualization.  
  - BLEU score tracking during training.  
- **Final Performance**:  
  - 0.46 BLEU score using **Moses multi-bleu.perl** on the test set.
    
🚀 **This project demonstrates an end-to-end Urdu-to-English translation pipeline using deep learning and attention mechanisms!**
