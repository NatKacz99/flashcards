# Flashcards Generator

An educational flashcards generator powered by Large Language Models such as Llama 3.2 and DeepSeek. The project uses Hugging Face Transformers, 4-bit quantization, and a Gradio interface to provide a simple and interactive user experience.

---

# Features

* Generate educational flashcards on any topic
* Support for multiple language models:

  * Llama 3.2 3B Instruct
  * DeepSeek R1 Distill Qwen 1.5B
* Interactive Gradio user interface
* 4-bit model loading with BitsAndBytes
* Markdown-based flashcard generation
* Adjustable number of generated flashcards

---

# Technologies

Built with:

* Python
* Hugging Face Transformers
* PyTorch
* BitsAndBytes
* Gradio
* Google Colab

---

# How It Works

1. The user enters a topic.
2. Selects a language model.
3. Chooses the number of flashcards.
4. The model generates question-answer flashcards in Markdown format.
5. Results are displayed inside the Gradio interface.

---

# Flashcard Format

Each flashcard is generated using the following structure:

```markdown
# Flashcard 1
<details>
<summary>What is the capital of France?</summary>
Paris
</details>
```

---

# Installation

## 1. Clone the repository

```bash
git clone https://github.com/your-username/flashcards-generator.git
cd flashcards-generator
```

## 2. Install dependencies

```bash
pip install -q --upgrade bitsandbytes accelerate
pip install transformers torch gradio huggingface_hub
```

---

# Configuration

The project requires a Hugging Face access token.

1. Create an account on Hugging Face.
2. Generate an API token.
3. Add the token as `HF_TOKEN` in Google Colab Secrets.

---

# Running the Project

Open the `flashcards.ipynb` notebook in Google Colab.

Run all notebook cells and launch the Gradio application.

---

# Example Usage

### Input

* Topic: `Machine Learning`
* Number of flashcards: `5`
* Model: `LLAMA`

### Output

```markdown
# Flashcard 1
<details>
<summary>What is supervised learning?</summary>
Learning using labeled data.
</details>
```

---

# Future Improvements

* Export flashcards to Anki
* Save generated flashcards to files
* Add support for more models
* Multilingual flashcard generation
* Streaming responses in the UI
* Deploy the application on Hugging Face Spaces
