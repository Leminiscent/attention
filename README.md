# Attention

This Python script leverages the power of the BERT (Bidirectional Encoder Representations from Transformers) model to visualize attention mechanisms. It offers an interactive experience, allowing users to input text with a masked token, which the model predicts. Additionally, the script generates diagrams visualizing the attention scores across different layers and heads of the model, providing insights into how BERT focuses on different parts of the input for its predictions.

## Features

- **Masked Language Model Prediction:** Uses a pre-trained BERT model to predict the word that fits in the place of a mask token within a given text.
- **Attention Visualization:** Generates diagrams for each attention head in each layer of the model, showcasing how words in the sentence attend to each other.

## Requirements

To run this script, ensure you have the following packages installed:

- `tensorflow` (Tested on 2.x)
- `transformers`
- `Pillow` (For image generation and manipulation)

Additionally, the script expects a font file located at `assets/fonts/OpenSans-Regular.ttf` for text rendering in the diagrams.

## Installation

1. Clone this repository or download the script.
2. Ensure you have Python 3.x installed.
3. Install the required Python packages using pip:

```sh
pip install tensorflow transformers Pillow
```

## Usage

Run the script from your command line:

```
python bert_attention_visualization.py
```

When prompted, enter your text with a mask token `[MASK]` included, e.g., `"The quick brown fox jumps over the lazy [MASK]."`

The script will output the top predictions for the masked word and generate attention visualization diagrams, which will be saved in the current directory.
