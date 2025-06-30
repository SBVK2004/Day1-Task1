# Day1-Task1
##Topic-Audio-based Anomaly Classifier

### Dataset - https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio

## ***objective***
#### The main goal of this project is to detect anomalies in a given audio 

## ***Steps for preprocessing of the audios***
 

| Step             | What It Does                           | Tool Used                                 |
| ---------------- | -------------------------------------- | ----------------------------------------- |
| Load audio files | Picks audio from RAVDESS               | `glob`, `librosa.load`, `IPython.display` |
| Trim silence     | Removes quiet parts                    | `librosa.effects.trim`                    |
| Plot waveform    | Shows amplitude over time              | `pandas`, `matplotlib`, `seaborn`         |
| Spectrogram      | Shows how frequencies change over time | `librosa.stft`, `librosa.display`         |
| Mel-spectrogram  | Human-like frequency perception        | `librosa.feature.melspectrogram`          |

## ***Tools/Libraries used***
| Tool/Library                 | Purpose                              |
| ---------------------------- | ------------------------------------ |
| **`pandas` / `numpy`**       | Data handling and arrays             |
| **`matplotlib` / `seaborn`** | Plotting graphs                      |
| **`librosa`**                | Audio analysis and processing        |
| **`IPython.display`**        | For playing audio inside notebook    |
| **`glob`**                   | For finding file paths from folders  |
| **`itertools.cycle`**        | For automatic color cycling in plots |

## ***Detecting Anamolies in the present audios***
| Stage              | Description                             |
| ------------------ | --------------------------------------- |
| Data Collection    | Used `glob` to fetch `.wav` files       |
| Labeling           | Used RAVDESS emotion codes to tag files |
| Feature Extraction | Used `librosa` MFCCs                    |
| Model Training     | Random Forest classifier                |
| Evaluation         | Accuracy + Confusion Matrix             |
| Inference          | Predict + Visualize + Play audio        |

## ***Tools/Libraries used***
| Library                 | Purpose                                             |
| ----------------------- | --------------------------------------------------- |
| `librosa`               | Load and process audio files, extract MFCC features |
| `pandas`, `numpy`       | Data manipulation                                   |
| `matplotlib`, `seaborn` | Visualizing waveforms and spectrograms              |
| `scikit-learn`          | Machine learning model (Random Forest)              |
| `glob`, `os`            | File handling (fetch all `.wav` files from folders) |
| `IPython.display`       | Play audio in notebook (Kaggle/Colab)               |




