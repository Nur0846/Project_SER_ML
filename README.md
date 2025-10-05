# 🎙️ Speech Emotion Recognition using IEMOCAP & CREMA-D — EmoNet Model

## Overview
This repository contains the implementation and experimental work corresponding to the conference paper:  
**“Speech Emotion Recognition using Dilated CNN-BiLSTM Network” (ECCE 2025)** by Md. Nur Alam.

The project focuses on building a robust **speech emotion recognition (SER)** system using **IEMOCAP** and **CREMA-D** datasets.  
It includes preprocessing, data balancing, augmentation, baseline modeling, and the development of the **EmoNet** model — a hybrid deep learning architecture combining **Dilated CNN** and **BiLSTM** layers to improve temporal and spectral emotion recognition.

---

## Key Features
- Multi-dataset training using **IEMOCAP** and **CREMA-D**  
- Feature extraction: MFCC and Log-Mel spectrograms  
- Data preprocessing: cleaning, balancing, and augmentation  
- Baseline model: *EmoTech* (CNN-BiLSTM hybrid)  
- Proposed model: *EmoNet* — combines Dilated CNN + BiLSTM for capturing short-term and long-range dependencies  
- Implemented in Python using TensorFlow/Keras

---

## Repository Structure
📁 Speech_Emotion_Recognition/
├── ECCE_2025_Speech_Emotion_Recognition_Nur.pdf # Conference paper
├── Paper_IEMOCAP.ipynb # Main notebook with code
├── README.md # This file


---

## Methodology

### 1. Data Preprocessing
- Combined IEMOCAP and CREMA-D datasets  
- Extracted **MFCC** and **Log-Mel** features  
- Applied **data balancing** to handle class imbalance  
- Performed **augmentation** including time-shifting, pitch scaling, and noise addition  

### 2. Baseline Model — EmoTech
A CNN-BiLSTM hybrid model serving as the initial benchmark. Focuses on sequential temporal learning but lacks global context.

### 3. Proposed Model — EmoNet
A **Dilated CNN + BiLSTM** network designed to capture both **short-term** and **long-range dependencies** in emotional speech.  
- Dilated convolutions expand context without losing resolution  
- BiLSTM layers model bidirectional temporal relationships  
- Dropout and BatchNorm layers improve stability and generalization  

---


---

## Author

**Md. Nur Alam**  
Department of Electronics and Telecommunication Engineering, CUET, Bangladesh  
📧 [nuralam1908046@gmail.com](mailto:nuralam1908046@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/nur-alam-4b664b219)


## Citation
If you use this work in your research, please cite:
```bibtex
@inproceedings{alam2025emotech,
  author    = {N. Alam and N. Mobassara and N. Mamun},
  title     = {Revamping EmoTech: Leveraging Dilated Convolution for Cutting-Edge Robust Speech Emotion Recognition},
  booktitle = {2025 International Conference on Electrical, Computer and Communication Engineering (ECCE)},
  year      = {2025},
  pages     = {1--6},
  address   = {Chittagong, Bangladesh},
  doi       = {10.1109/ECCE64574.2025.11013956},
  keywords  = {Emotion recognition, Accuracy, Convolution, Bidirectional long short term memory, Speech recognition, Data augmentation, Feature extraction, Data models, Robustness, Mel frequency cepstral coefficient, Speech Emotion Recognition, Dilated Convolution, BiLSTM, MFCC}
}

