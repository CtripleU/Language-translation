# English to Igbo Neural Machine Translation

This project implements a neural machine translation model to translate English sentences to Igbo using a sequence-to-sequence LSTM architecture. The model is trained on a dataset of English-Igbo sentence pairs and achieves high accuracy in translation tasks.

## Features

- Utilizes a sequence-to-sequence LSTM model for translation
- Implements data preprocessing techniques for text cleaning
- Uses TensorFlow and Keras for model building and training
- Achieves high accuracy on both training and validation sets

## Dataset

The project uses the "english_to_igbo" dataset from Hugging Face:

- Source: ccibeekeoc42/english_to_igbo
- Total samples: 525,618 (522,322 train, 3,296 test)
- Features: 'English' and 'Igbo' sentence pairs

For this project, I sampled 10,000 rows from the training dataset to reduce computational requirements.

## Installation

1. Clone the repository:
```
git clone https://github.com/yourusername/english-to-igbo-translation.git
cd english-to-igbo-translation
```

2. Install the required packages:
```
pip install tensorflow pandas sklearn nltk datasets
```

## Usage

Run the Jupyter notebook or Python script to:

1. Load and preprocess the dataset
2. Build and train the sequence-to-sequence model
3. Evaluate the model on the test set
4. Generate translations for new English sentences

## Model Architecture

The model uses a sequence-to-sequence architecture with:

- Encoder: LSTM with 512 units
- Decoder: LSTM with 512 units
- Embedding layer: 256-dimensional embeddings
- Dense output layer with softmax activation

Total params: 13,571,229 (51.77 MB)

## Results

After training for 20 epochs:

- Training Accuracy: 100.00%
- Validation Accuracy: 98.10%
- Test Accuracy: 94.71%
- Test Loss: 0.4220


## Future Work

- Experiment with transformer-based architectures
- Increase dataset size and diversity
- Implement beam search for improved translation quality
- Add attention mechanism to the model

## Acknowledgments

- The creators of the "english_to_igbo" dataset on Hugging Face
- TensorFlow and Keras documentation and community

## License

This project is licensed under the MIT License.
