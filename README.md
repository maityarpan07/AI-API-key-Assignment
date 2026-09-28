# Generative AI API Experiments

This repository contains three Google Colab notebooks demonstrating how to call different large language models (LLMs) through Python APIs and generate text responses from user prompts.

## Notebooks

### 1. `Gemini.ipynb`

This notebook demonstrates text generation using the Google Gemini API.

**Main steps:**
1. Install the `google-genai` package.
2. Retrieve the `GEMINI_API_KEY` from Google Colab User Secrets.
3. Create a Gemini client.
4. Send a text prompt to the Gemini model.
5. Print the generated response.

**Model used:**
- `gemini-3.8-flash`

**Example prompt:**
> The closest habitble planet in our galaxy acording to scientists in one line answer

---

### 2. `OpenAI.ipynb`

This notebook demonstrates text generation through the Groq API using a Qwen model.

**Main steps:**
1. Install the `groq` package.
2. Retrieve the `GROQ_API_KEY` from Google Colab User Secrets.
3. Create a Groq client.
4. Send a chat-completion request.
5. Print the generated response.

**Model used:**
- `qwen/qwen3.8-27b`

**Example prompt:**
> what is the largest continet and what is the approx population in numbers

---

### 3. `OpenAI_2.ipynb`

This notebook demonstrates text generation through the Groq API using an OpenAI GPT-OSS model.

**Main steps:**
1. Install the `groq` package.
2. Retrieve the `GROQ_API_KEY` from Google Colab User Secrets.
3. Create a Groq client.
4. Send a chat-completion request.
5. Print the generated response.

**Model used:**
- `openai/gpt-oss-120b`
- The notebook also mentions `openai/gpt-oss-20b` as an alternative.

**Example prompt:**
> give me a list of animals are going to be extincted in future

## Requirements

The notebooks are designed to run in Google Colab.

Required Python packages:

```bash
pip install google-genai
pip install groq
```

## API Keys

The notebooks use API keys stored in **Google Colab User Secrets**.

Required secrets:

- `GEMINI_API_KEY` for `Gemini.ipynb`
- `GROQ_API_KEY` for `OpenAI.ipynb`
- `GROQ_API_KEY` for `OpenAI_2.ipynb`

Do not hard-code or publicly share your API keys.

## How to Run

1. Open the required `.ipynb` file in Google Colab.
2. Add the required API key to Google Colab **Secrets**.
3. Enable notebook access to the secret.
4. Run the cells from top to bottom.
5. The generated model response will be displayed below the final cell.

## Project Workflow

```text
Install required package
        ↓
Load API key from Colab Secrets
        ↓
Create API client
        ↓
Select AI model
        ↓
Send user prompt
        ↓
Generate response
        ↓
Print response
```

## Technologies Used

- Python
- Google Colab
- Google GenAI API
- Groq API
- Gemini
- Qwen
- OpenAI GPT-OSS

## Purpose

The notebooks provide simple examples of connecting Python applications to generative AI models and generating text responses from natural-language prompts. They can serve as introductory experiments for understanding API-based LLM usage.

## Notes

The README describes the notebooks as they are currently implemented. Each notebook contains a single example prompt and prints the resulting model response.
