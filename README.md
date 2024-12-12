# Classifying Emotional States Through EEG-Derived Spectrograms

## Introduction
This repository contains the code and resources for the project **Classifying Emotional States Through EEG-Derived Spectrograms**, developed by Team Scalar as part of the EmoNeuroDB competition hosted by [Voxellab](https://voxellab.pl/EmoNeuroDB/). The project was also presented at the **2024 IEEE 18th International Conference on Automatic Face and Gesture Recognition (FG)**, where it was published as a conference paper.

## Competition Overview
The EmoNeuroDB competition focuses on using EEG data to classify emotional states. The dataset comprises EEG recordings from multiple participants experiencing various emotions. These signals are essential for exploring affective computing, healthcare applications, and improving human-computer interaction systems.

Competition link: [EmoNeuroDB](https://voxellab.pl/EmoNeuroDB/)

## Our Contribution
Our project explored the feasibility of classifying six human emotions (fear, anger, joy, disgust, surprise, and sadness) using EEG data. To achieve this, we:

- Preprocessed EEG time-series data and converted it into spectrograms.
- Developed and tested machine learning and deep learning models, including Random Forest, KNN, 2D CNN, 3D CNN, and sequence models (RNN, LSTM, and their bidirectional counterparts).
- Compared sequential models with image processing approaches for the classification task.
- Achieved our best results using the KNN model during the test phase.

## Publication
Our findings were published in the following conference paper:

**[Classifying Emotional States Through EEG-Derived Spectrograms](https://ieeexplore.ieee.org/document/10581899)**  
A D Mahit Nandan, Dhiraj Choudhary D, Ishan Godbole, and Anand Kumar M  
*2024 IEEE 18th International Conference on Automatic Face and Gesture Recognition (FG)*  

### Citation
If you use our work, please cite:
```bibtex
@INPROCEEDINGS{10581899,
  author={Mahit Nandan, A D and D, Dhiraj Choudhary and Godbole, Ishan and M, Anand Kumar},
  booktitle={2024 IEEE 18th International Conference on Automatic Face and Gesture Recognition (FG)},
  title={Classifying Emotional States Through EEG-Derived Spectrograms},
  year={2024},
  pages={1-5},
  keywords={Time series analysis;Sociology;Mental health;Medical services;Brain modeling;Data models;User experience},
  doi={10.1109/FG59268.2024.10581899}
}
```

## Dataset
We used the **EmoNeuroDB EEG dataset**, which includes recordings from 40 participants (24 males, 16 females) aged 19-57. Each participant was exposed to six emotions, with EEG signals recorded for 15 seconds per emotion.

### Key Details:
- EEG headset: DSI-24, a wireless research-grade dry electrode EEG device.
- Data resolution: 4500 time points per sample, recorded every 3.33 milliseconds.
- Features: 24 brain regions, including Fp1, Fp2, F3, F4, C3, C4, etc.

The dataset was split into training and testing sets in a 2:1 ratio.

## Methodology
1. **Data Preprocessing:** Standardization and feature engineering of EEG signals.
2. **Machine Learning Approaches:** Implemented Random Forest and KNN models.
3. **Deep Learning Approaches:** Developed 2D and 3D CNNs using spectrograms.
4. **Sequence Models:** Utilized RNNs and LSTMs for time-series analysis.

## Results
| Model            | Overall Accuracy |
|------------------|------------------|
| Random Forest    | 17.78%           |
| KNN              | 25.56%           |
| 2D CNN           | 26.67%           |
| 3D CNN           | 25.00%           |
| LSTM             | 22.00%           |

Our best-performing model, KNN, demonstrated effective generalization across unseen data.

## Future Work
We plan to enhance classification performance by:
- Applying transformer-based models for image analysis.
- Exploring advanced feature extraction techniques for spectrograms.

## Team
- **A D Mahit Nandan**  
- **Dhiraj Choudhary D**  
- **Ishan Godbole**  
- **Anand Kumar M**  

Affiliation: National Institute of Technology Karnataka (NITK), Department of Information Technology

## Contact
For any questions or collaborations, please reach out via the competition platform or contact the authors.

---

Thank you for exploring our project!
