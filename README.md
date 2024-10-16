# LaTeX to Python Code Converter

This project focuses on converting mathematical expressions written in LaTeX into executable Python code. We fine-tune a pre-trained transformer-based model on a custom synthetic dataset of LaTeX expressions and their corresponding Python code.

The goal is to allow automated translation of complex mathematical formulas into Python code, making it easier for users to execute or analyze mathematical expressions programmatically.

## Dataset

The dataset used for training consists of synthetic examples that pair LaTeX expressions with their equivalent Python code. The dataset contains various types of mathematical expressions including:

- **Multivariable equations**
- **Trigonometric functions**
- **Geometric expressions**
- **Diophantine equations**
- **Summations**
- **Differentiation equations**
- **Exponential equations**
- **Quadratic equations**
- **Integration equations**
- **Logarithmic equations**
- **Algebraic equations**
- **Derivatives**

### Data Access

The training data is provided in a zipped format (`train.zip`). To use the dataset, unzip the file.

## Training the Model

To fine-tune the model on the dataset, you can use the provided `train.py` script:

```bash
python train.py
```

This will fine-tune the model using the training data, allowing the model to learn the mapping from LaTeX expressions to Python code.

## Inference

To convert a LaTeX expression into Python code using the fine-tuned model, run the `inference.py` script:

```bash
python inference.py
```

The model will output the corresponding Python code for the provided LaTeX expression.

## Testing the Model on Hugging Face Space

You can also test the model on Hugging Face without installing anything. Visit our Hugging Face Space to try out the LaTeX-to-Python conversion app:

[https://huggingface.co/spaces/sabssag/Latex_to_Python_CodeT5-base](#)

Simply enter a LaTeX expression, and the model will generate the equivalent Python code.

## Requirements

To set up the environment and install dependencies, use the provided `requirements.txt`:

```bash
pip install -r requirements.txt
```

## Future Directions

We plan to improve the dataset by expanding the variety of expressions and optimizing the model for faster and more accurate conversions. Feel free to contribute by providing feedback or opening issues.
