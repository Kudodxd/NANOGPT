# NANOGPT Project

*NANOGPT* is a deep learning project that implements a character-level bigram language model and supporting utilities for CUDA-accelerated computations using PyTorch.

## Project Structure

- **[bigram.py](bigram.py)**  
  Implements a simple bigram language model. This file includes text preprocessing, model definition, training loop, evaluation functions, and text generation routines using an embedding-based approach.

- **[check_cuda.py](check_cuda.py)**  
  A utility script to verify your PyTorch installation and CUDA support. It prints the PyTorch version and whether CUDA is available.

- **[more.txt](more.txt)**  
  Contains Shakespeare-inspired text that can be used either for testing text generation or for further experiments in text analysis.

- **input.txt**  
  The text file containing the training data (e.g., Tiny Shakespeare), which is loaded in the scripts.

## Requirements

- **Python:** 3.8 or higher  
- **PyTorch:** Installed with CUDA support  
- **CUDA:** A compatible GPU and the appropriate driver/CUDA toolkit

## Set Up a Virtual Environment

### On Windows (Command Prompt or PowerShell):
```bash
python -m venv venv
.\venv\Scripts\activate
```

### On Unix or macOS:
```bash
python3 -m venv venv
source venv/bin/activate
```

## Install Dependencies

Install PyTorch with CUDA support. For example, for CUDA 11.7:
```bash
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu117
```

If you have additional dependencies, install them via:
```bash
pip install -r requirements.txt
```

## Usage

### Training and Text Generation

Run the bigram model script to train or generate text:
```bash
python bigram.py
```

### Verify CUDA Installation

Check your PyTorch and CUDA setup with the utility script:
```bash
python check_cuda.py
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.
