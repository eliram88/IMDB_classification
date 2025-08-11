# IMDB Movie Review Sentiment Classification

🎯 هدف پروژه: طبقه‌بندی نظرات کاربران دیتاست IMDB به دو دسته مثبت و منفی  در TensorFlow/Keras.


## 🌐 لینک ها

- [دیتاست پروژه](https://storage.googleapis.com/tensorflow/tf-keras-datasets/imdb.npz)
  فایل دیتاست مورد استفاده در پروژه

- [مشاهده پروژه در Google Colab](https://colab.research.google.com/drive/1zYiy6fIgYLUgisngQR40IXt8h_83vNBR?usp=sharing)
 اجرای آنلاین کد پروژه در محیط Google Colab

- [مشاهده پروژه در GitHub](https://github.com/eliram88/IMDB_Classification)
  سورس کد و مستندات پروژه در GitHub



## 🔧 ابزارهای استفاده‌شده

- Python (Numpy, Tensorflow, Matplolib, Keras)
- Google Colab
- Google Drive
- GitHub for version control



## 📊 Dataset | دیتاست

- **Source:** IMDB dataset from `keras.datasets`
- **Samples:** 50,000 movie reviews  
  - 25,000 for training  
  - 25,000 for testing  
- **Labels:**  
  - `0` → Negative  
  - `1` → Positive  



## 📊 مراحل پروژه

### 🛠 Preprocessing | پیش‌پردازش

- Vectorizing Text Sequences for Neural Network Input
(هر نقد که به صورت لیستی از اندیس کلمات است، به یک وکتور باینری تبدیل میشود)


### 🧠 Model Design | طراحی مدل

- MLP (Multi-Layer Perceptron):

    Input Layer → 10,000 features
    Dense Layer → 16 units, relu activation
    Dense Layer → 16 units, relu activation
    Output Layer → 1 unit, sigmoid activation (for binary classification)


### ⚙ Training | آموزش

    Optimizer: RMSprop
    Loss: Binary Crossentropy
    Metric: Accuracy
    Batch Size: 512
    Epochs: 20 


### 📈 Results | نتایج

    Validation Accuracy: ~86%
    Test Accuracy: ~87%
    Validation Loss Curve: loss decreases steadily until overfitting after ~4 epochs.



## 🚀 How to Run | نحوه اجرا

1) Install dependencies | نصب کتابخانه‌ها
```bash
pip install tensorflow numpy matplotlib
```

2) Run Jupyter Notebook | اجرای نوت‌بوک
```bash
jupyter notebook
```
Open the file IMDB_Classification.ipynb and run all cells.



## 📁 ساختار فایل‌ها
```bash
IMDB_Classification/
│
├── 📁 notebook/
│   └── IMDB_Classification.ipynb     # Data analysis & model training
│
├── 📄 README.md                      # Project documentation
```



## 🧑‍💻 توسعه‌دهنده

این پروژه توسط یک علاقه‌مند به تحلیل داده و یادگیری ماشین طراحی و اجرا شده  
با هدف شرکت در موقعیت های "تحلیلگر داده / دیتا ساینتیست".

✨ هدف: توسعه نمونه کار قابل ارائه، تمرین تحلیل واقعی، یادگیری مدل‌سازی حرفه‌ای و تفسیر مدل
