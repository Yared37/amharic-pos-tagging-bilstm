#  Amharic Part-of-Speech Tagging Using BiLSTM

This project implements a **Part-of-Speech (POS) tagging model for the Amharic language** using a **Bidirectional Long Short-Term Memory (BiLSTM)** neural network.  
It aims to advance **Natural Language Processing (NLP)** research for low-resource languages, particularly Amharic — one of the most widely spoken languages in Africa.

---

##  Overview

Part-of-Speech tagging is a fundamental task in NLP that assigns grammatical labels (e.g., noun, verb, adjective) to words in a sentence.  
While English and other major languages benefit from extensive datasets and pre-trained models, **Amharic lacks robust open-source POS taggers**.  
This project bridges that gap by training a deep learning model specifically designed for Amharic text.

---

##  Model Architecture

The model uses a **BiLSTM** network to capture both past and future context of words in a sentence.  
This bidirectional nature allows the model to understand how surrounding words influence a token’s grammatical role.

**Model Pipeline:**
1. Text preprocessing and tokenization  
2. Word embedding representation  
3. BiLSTM layers for context understanding  
4. Dense output layer with softmax activation for tag prediction  

**Framework:** TensorFlow   
**Language:** Python  

---

##   Dataset

- **Source:** Amharic tagged corpus (mention your dataset if public, e.g. “the Amharic POS dataset from the Ethiopian NLP research group”).  
- **Format:** Each sentence is tokenized with corresponding POS labels.  
- **Preprocessing:** Text normalization, token encoding, and sequence padding.  


---

##   Evaluation

The model’s performance is measured using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**

Results demonstrate strong performance in capturing linguistic patterns unique to Amharic morphology and syntax.

---

##   Example Output

**Input Sentence:**  
> አባቴ ቤት ሄደ።  

**Predicted POS Tags:**  
> አባቴ → Noun  
> ቤት → Noun  
> ሄደ። → Verb  
