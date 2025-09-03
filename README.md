# IMDB Movie Review Sentiment Classification

🎯 Project goal: Classify IMDB movie reviews into positive and negative categories using TensorFlow/Keras.


## 🌐 Links

- [Dataset](https://storage.googleapis.com/tensorflow/tf-keras-datasets/imdb.npz)  
  IMDB Dataset

- [View project in Google Colab](https://colab.research.google.com/drive/1zYiy6fIgYLUgisngQR40IXt8h_83vNBR?usp=sharing)  
   Google Colab Notebook: Run the project online

- [View project in GitHub](https://github.com/eliram88/IMDB_Classification)  
  GitHub Repository: Source code & documentation


## 🔧 Tools & Libraries

- Python (Numpy, Tensorflow, Matplolib, Keras)
- Google Colab
- Google Drive
- GitHub for version control



## 📊  Dataset

- **Source:** IMDB dataset from `keras.datasets`
- **Samples:** 50,000 movie reviews  
  - 25,000 for training  
  - 25,000 for testing  
- **Labels:**  
  - `0` → Negative  
  - `1` → Positive  



## 📊 Project Stages

### 🛠 Preprocessing 

- Vectorized text sequences for neural network input
- Each review (as a list of word indices) was transformed into a binary vector representation


### 🧠 Model Design

- MLP (Multi-Layer Perceptron):

   - Input Layer → 10,000 features
   - Dense Layer → 16 units, relu activation
   - Dense Layer → 16 units, relu activation
   - Output Layer → 1 unit, sigmoid activation (for binary classification)


### ⚙ Training 
 
 - Optimizer: RMSprop
 - Loss: Binary Crossentropy
 - Metric: Accuracy
 - Batch Size: 512
 - Epochs: 20 


### 📈 Results 

- Validation Accuracy: ~86%
- Test Accuracy: ~87%
- Validation Loss Curve: loss decreases steadily until overfitting after ~4 epochs.



## 🚀 How to Run

1) Install dependencies 
```bash
pip install tensorflow numpy matplotlib
```

2) Run Jupyter Notebook
```bash
jupyter notebook
```
Open the file IMDB_Classification.ipynb and run all cells.



## 📁 Project Structure
```bash
IMDB_Classification/
│
├── 📁 notebook/
│   └── IMDB_Classification.ipynb     # Data analysis & model training
│
├── 📄 README.md                      # Project documentation
│
├── requirements.txt		              # Project Libraries
```



## 🧑‍💻 Developer

This project was developed by a data analysis and machine learning enthusiast with the goal of:

- Practicing text classification with neural networks
- Building a professional portfolio project
- Gaining expertise in interpreting models for sentiment analysis
