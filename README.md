
## 📖 Description

When working with LLMs like GPT-4o-mini, the `temperature` parameter is one of the most important settings to understand. This project walks through what temperature means, how it affects model output, and shows real side-by-side examples to make the concept intuitive.

**In short:**
- **Low temperature (e.g., 0)** → Safe, predictable, consistent outputs
- **High temperature (e.g., 2)** → Creative, surprising, sometimes chaotic outputs

---

## 🧠 Concepts Covered

- What temperature is and how it works internally
- How low temperature produces near-deterministic responses
- How high temperature leads to highly varied (and sometimes incoherent) responses
- Practical intuition: "picking words from a list"

---

## 🗂️ Project Structure

```
├── understanding_temperature_use.ipynb   # Main notebook with examples
└── keys/
    └── .openai_api_key.txt               # Your OpenAI API key (not included)
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab
- An OpenAI API key

### Installation

```bash
pip install openai jupyter
```

### Setup

1. Clone or download this repository.
2. Create a `keys/` directory in the project root.
3. Add your OpenAI API key to `keys/.openai_api_key.txt`.

```bash
mkdir keys
echo "your-api-key-here" > keys/.openai_api_key.txt
```

4. Launch the notebook:

```bash
jupyter notebook understanding_temperature_use.ipynb
```

---

## 🔬 Experiments in the Notebook

| Temperature | Behavior | Example Output |
|-------------|----------|----------------|
| `0` | Deterministic, consistent | Clean, structured poem repeated across runs |
| `2` | Highly random | Garbled, multilingual, or nonsensical output |

The notebook runs the same prompt — *"write a poem on India in 5 lines"* — multiple times at each temperature setting, so you can directly compare the outputs.

---

## ⚠️ Notes

- A temperature of `2` is at the extreme end of the scale and is used here purely for demonstration. For most real-world tasks, values between `0` and `1` are recommended.
- Keep your API key private — never commit `keys/.openai_api_key.txt` to version control. Add it to `.gitignore`.

---

## 📄 License

This project is for educational purposes. Feel free to use and modify it as needed.
