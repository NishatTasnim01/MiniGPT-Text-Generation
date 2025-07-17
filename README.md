# 🧠 MiniGPT-Text-Generation

A lightweight implementation of a GPT-style Transformer model built from scratch using PyTorch. This project demonstrates how to train a mini language model capable of generating coherent text sequences based on input prompts. The model uses a custom-built transformer encoder and is trained on plain text files.


## 🚀 Features

- GPT-style Transformer architecture
- Tokenization with HuggingFace GPT-2 tokenizer
- Custom dataset and dataloader for next-token prediction
- Training loop with loss reporting and text generation
- Text generation using temperature-controlled sampling

## 📂 Project Structure

```bash
MiniGPT-Text-Generation/
│
├── harry\_potter.txt              # Input training text file
├── gpt2_text_generator.ipynb      # Training and inference code
└── README.md                      # Project documentation
```

## 📖 How It Works

1. **Load text data**  : Reads raw text from a `.txt` file.

2. **Tokenization**  : Uses the pretrained GPT-2 tokenizer from HuggingFace.

3. **Data Preparation**  : Chunks the tokenized text into fixed-length sequences and prepares them for next-token prediction.

4. **MiniGPT Model**  : Implements a simple Transformer-based language model with embedding, positional encoding, and multi-layer encoder blocks.

5. **Training Loop**  : Uses cross-entropy loss and the Adam optimizer to minimize prediction error.

6. **Text Generation**  : Generates new text sequences from a starting prompt using temperature-scaled sampling.

## 🛠️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/NishatTasnim01/MiniGPT-Text-Generation.git
cd MiniGPT-Text-Generation
````

### 2. Install Dependencies
```bash
pip install torch transformers pypdf2
```
> 🔍 **Note**: `PyPDF2` is optional and used only if you're loading data from a `.pdf`.

## 🧪 Usage

1. Place your training `.txt` file (e.g., `harry_potter.txt`) in the root directory.
2. Run the notebook or script to train the model:

   ```bash
   python gpt2_text_generator.ipynb
   ```
3. The script will train for 500 epochs and generate sample text every 10 epochs.


## 📌 Requirements

* Python 3.7+
* PyTorch
* Transformers (HuggingFace)
* PyPDF2 (for optional text loading from PDFs)

## 📚 Dataset

Any `.txt` file containing plain English text can be used. Example used:

* *Harry Potter and the Sorcerer's Stone (Text Version)*

## 🌟 Show Your Support

If you found this project helpful, please ⭐️ star the repo and share it with others!
