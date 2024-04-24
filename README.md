# Enhancing Stable Diffusion for Gaming Characters

<br>

## Introduction

Welcome to our project dedicated to enhancing Stable Diffusion, an advanced neural network designed for generating high-quality images. Our goal is to optimize Stable Diffusion by fine-tuning it with gaming asset datasets, allowing for the creation of compelling character artworks.

Stable Diffusion, introduced in 2022, is a powerful deep learning model based on diffusion techniques. Initially developed for generating detailed images from text descriptions, it has since found applications in various tasks such as image completion, expansion, and guided image synthesis (Wikipedia contributors, 2024).

<br>

## Getting Started

### Requirements

- Python 3.9+
- Installation of required dependencies listed in "requirements.txt".
```
pip install -r requirements.txt
```


<br>

## Data Preparation

To prepare your data for fine-tuning the Stable Diffusion model, follow these simple steps:

### Step 1: Organize Your Image Dataset

Place all desired images for fine-tuning in the ./data/images/ directory.

### Step 2: Writing Prompts for Images

- Single Prompt (for Dreambooth): Define a single clear prompt for fine-tuning all images.
- Multiple Prompts (for Keras-CV): Generate individual prompts for each image using the BLIP model via the ./preparation/auto prompting using BLIP.ipynb script.




<br>

## Fine-Tuning Process

### Using Dreambooth

Fine-tune the Stable Diffusion model using Dreambooth. This involves configuring the model from the huggingface repository and training it with gaming character datasets. The fine-tuned model is then utilized to generate new artworks featuring gaming characters.


### Employing Keras-CV

Fine-tune the Stable Diffusion model using TensorFlow's Keras framework. A custom class manages the training procedures, including loss computation and gradient updates, thereby refining parts of the diffusion model.





<br>

## Evaluation

The fine-tuned Stable Diffusion model has produced a collection of character images for evaluation, demonstrating its proficiency in:

- Ensuring the presence of requested objects in each image.
- Exhibiting variation in character designs, encompassing diverse shapes and colors.
- Simplifying backgrounds for clarity and focus.
- Clearly distinguishing characters from their backgrounds.

### Character Variation

<table align="center">
  <tr>
    <td><img src="https://raw.githubusercontent.com/SoheilMohammadpour231754/Stable-Diffusion/main/generated%20artworks/dreambooth/a%20demon%20dressed%20in%20red%20and%20holding%20a%20sword.png" alt="Demon with sword" width="200"></td>
    <td><img src="https://raw.githubusercontent.com/SoheilMohammadpour231754/Stable-Diffusion/main/generated%20artworks/dreambooth/Elfs%20with%20arrows.png" alt="Elfs with arrows" width="200"></td>
    <td><img src="https://raw.githubusercontent.com/SoheilMohammadpour231754/Stable-Diffusion/main/generated%20artworks/dreambooth/Gandalf%20the%20gray.png" alt="Gandalf the gray" width="200"></td>
  </tr>
  <tr>
    <td align="center">A demon</td>
    <td align="center">Two elves</td>
    <td align="center">A wizard</td>
  </tr>
</table>

### Colour Variation of Same Characters

<table align="center">
  <tr>
    <td><img src="https://raw.githubusercontent.com/SoheilMohammadpour231754/Stable-Diffusion/main/generated%20artworks/dreambooth/Knights%20in%20blue%2C%20black%20and%20white%20with%20an%20elaborate%20helmet%20on%20their%20head.png"  width="200"></td>
    <td><img src="https://raw.githubusercontent.com/SoheilMohammadpour231754/Stable-Diffusion/main/generated%20artworks/dreambooth/Knights%20in%20red%2C%20black%20and%20white%20with%20an%20elaborate%20helmet%20on%20their%20head.png" width="200"></td>
    <td><img src="https://raw.githubusercontent.com/SoheilMohammadpour231754/Stable-Diffusion/main/generated%20artworks/dreambooth/Knights%20in%20green%2C%20black%20and%20white%20with%20an%20elaborate%20helmet%20on%20their%20head.png" width="200"></td>
  </tr>
  <tr>
    <td align="center">Blue knights</td>
    <td align="center">Red knights</td>
    <td align="center">Green knights</td>
  </tr>
</table>


