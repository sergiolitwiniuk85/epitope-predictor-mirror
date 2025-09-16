# epitope-predictor-mirror

````
# Epitope Predictor Mirror

<p align="center">
  <a href="https://huggingface.co/spaces/sergiolitwiniuk/epitope-predictor">
    <img src="https://img.shields.io/badge/Hugging%20Face%20Space-Deployed-blue?style=for-the-badge&logo=huggingface" alt="Hugging Face Space">
  </a>
  <a href="https://huggingface.co/sergiolitwiniuk/adapter-esm2-150M">
    <img src="https://img.shields.io/badge/Hugging%20Face%20Model-Adapter-orange?style=for-the-badge&logo=huggingface" alt="Hugging Face Model">
  </a>
</p>

---

## 🧐 About this Project

This repository serves as a **"mirror"** (replica) of the **Epitope Predictor** project, a biological language model fine-tuned for epitope prediction. The model uses an `Esm2-150M` adapter to identify amino acid sequences likely to form an epitope—the part of a molecule recognized by the immune system.

The goal of this repository is to provide a backup and an alternative access point to the model and its associated scripts, ensuring the project is accessible and easy to replicate.

## 🚀 Resources and Links

All the main components of the project are available on the Hugging Face platform:

- **Hugging Face Space (Interactive Demo)**: You can interact with the model directly through the web interface at the following link:
  - [**sergiolitwiniuk/epitope-predictor**](https://huggingface.co/spaces/sergiolitwiniuk/epitope-predictor)

- **Adapter Model**: The fine-tuned model (`adapter-esm2-150M`) is hosted on the Hugging Face Hub, where it can be downloaded and used in your own projects:
  - [**sergiolitwiniuk/adapter-esm2-150M**](https://huggingface.co/sergiolitwiniuk/adapter-esm2-150M)

## 💻 Local Usage

To use the model locally, clone this repository and ensure you have the necessary dependencies.

### 1. Clone the Repository

```bash
git clone [https://github.com/your_username/epitope-predictor-mirror.git](https://github.com/your_username/epitope-predictor-mirror.git)
cd epitope-predictor-mirror
````

### 2\. (Optional) Install Dependencies

If the project has a `requirements.txt` file, you can install the dependencies with:

```bash
pip install -r requirements.txt
```

### 3\. Load the Model

You can load the model and adapter in Python using the Hugging Face `transformers` library.

```python
from transformers import AutoModelForMaskedLM, AutoTokenizer
from peft import PeftModel

# Load the base model
model_name = "facebook/esm2_t6_8M_UR50D"
model = AutoModelForMaskedLM.from_pretrained(model_name)
tokenizer = AutoTokenizer.from_pretrained(model_name)

# Load the adapter from the repository
adapter_model = PeftModel.from_pretrained(model, "sergiolitwiniuk/adapter-esm2-150M")

# Now you can use the 'adapter_model' for inference
```

## 📜 License

This project is distributed under the [**MIT License**](https://opensource.org/licenses/MIT).

-----

```
```
