# uk-to-us-converter
This repository contains a T5-based NLP model that converts UK English spelling and phrasing into US English. Built using PyTorch and the Hugging Face Transformers library, the model is trained to recognize and translate British spelling differences into their American equivalents.

#Installation

To run this code, you will need to install the following dependencies:

!pip install transformers datasets torch accelerate

#Usage

1.Clone the repository:

git clone <your-repo-url>

cd uk-to-us-converter

2.Train the model using your own dataset by running the uk_to_us_converter.ipynb notebook.

3.Save the model using:

model.save_pretrained("uk_us_translator")

tokenizer.save_pretrained("uk_us_translator")

4.To use the model for prediction:

translated_text = translate("I travelled to the centre of the city.", model, tokenizer, device)

print(translated_text)  
# Output: 
"I have an apartment near the elevator."

#Example

Input: "I have a flat near the lift."

Output: "I have an apartment near the elevator."
