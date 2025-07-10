#  IE Hackathon 2023

A Python-based CLI tool designed for processing document directories using OpenAI GPT models (GPT‑3.5-turbo or GPT‑4). It analyzes files in a dataset folder and generates a structured output CSV—ideal for hackathon submissions or quick prototyping.

---

## Features

* 📂 Processes all documents in a given dataset directory
* 🛠 Supports GPT‑3.5 and GPT‑4 (use `--gpt4` for better results)
* 📝 Outputs structured data (e.g., CSV) for downstream analysis
* 🧠 Includes modular components for RAG, text comparison, and processing

---

## Prerequisites

* Python 3.11.5
* OpenAI API key (set as environment variable `OPENAI_API_KEY`)

---

## Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/ayayasminebelloum/ie-hackathon-2023.git
cd ie-hackathon-2023
pip install -r requirements.txt
```

---

## Usage

Run the main processing script:

```bash
python main.py <dataset_dir> <output_file.csv> [--gpt4]
```

* `<dataset_dir>`: Directory with all input documents
* `<output_file.csv>`: Destination CSV file for processed results
* `--gpt4`: (Optional) Use GPT‑4 instead of GPT‑3.5-turbo

### Example

```bash
python main.py ./data ./results/out.csv --gpt4
```

---

## Repository Structure

* `main.py` – Entry point, orchestrates processing workflow
* `compare.py` – Utilities for document/content comparison
* `clai.py` – OpenAI client and prompt handling
* `rag.py` – Retrieval-Augmented Generation methods
* `requirements.txt` – Project dependencies

---

## Contribution

Feel free to open issues or submit pull requests. Suggestions welcome for:

* Batch processing enhancements
* Support for additional output formats (JSON, Excel, etc.)
* CLI flags for logging, verbosity, otherwise

---

## 📄 License

This project is currently unlicensed. If you'd like to open-source it under MIT, Apache 2.0, or another license, just add a `LICENSE` file.

---

### Summary

This tool provides an easy-to-use command-line interface to process document collections with OpenAI GPT models, producing formatted outputs for data analysis, automation, or hackathon challenges. Use it as a foundation or extend it to fit your use cases!
