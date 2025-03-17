# Shakespeare Text Generation with LSTM  

This project trains a neural network to generate Shakespeare-style text using a Long Short-Term Memory (LSTM) model.  

## Features  
- Downloads Shakespeare's complete works.  
- Preprocesses the text data for character-level prediction.  
- Trains an LSTM-based neural network to predict the next character in a sequence.  
- Generates new text samples based on learned patterns.  

## Requirements  
Ensure you have the following dependencies installed:  

- Python 3.x  
- TensorFlow  
- NumPy  
- Pandas  

You can install them using:  

```bash  
pip install tensorflow numpy pandas  
```  

## Usage  

### 1. Clone the repository  
```bash  
git clone https://github.com/yourusername/shakespeare-lstm.git  
cd shakespeare-lstm  
```  

### 2. Run the Notebook  
Open the Jupyter Notebook (`SHAKESPEARE.ipynb`) or execute the script in Google Colab.  

### 3. Model Training  
The script:  
- Loads Shakespeare's text from TensorFlow datasets.  
- Processes the text into sequences for training.  
- Builds an LSTM model and trains it using character-level prediction.  

### 4. Generating Text  
The `generate_text(length, temperature)` function generates text using the trained model.  
Adjusting the **temperature** parameter influences randomness:  
- **Lower temperature** (e.g., `0.2`) → More predictable, structured text.  
- **Higher temperature** (e.g., `0.8`) → More creative, but riskier outputs.  

## Example Output  
```
----0.2----  
him say so then, and let him go;  
but let  
```  

## Notes  
- Training may take time depending on system performance.  
- Results improve with more epochs and fine-tuned hyperparameters.  

## License  
This project is open-source and free to use under the MIT License.  
