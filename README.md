# Text-to-Code Generation

## 📌 Project Overview
The **Text-to-Code Generation** project is an advanced AI-driven system that converts natural language descriptions into executable code in multiple programming languages, including **Python, C++, Java, and PHP**. This project leverages a **Large Language Model (LLM)** to generate accurate and context-aware code snippets based on user input.

## 🚀 Features
- **Multi-language support:** Generates code in Python, C++, Java, and PHP.
- **Transformer-based architecture:** Utilizes "EleutherAI/gpt-neo-2.7B" for text-to-code conversion.
- **Model optimization:** Implements **Quantization** (INT4) to reduce model size and improve efficiency.
- **Fine-tuning with LoRA:** Uses **Low-Rank Adaptation (LoRA)** to fine-tune the model without modifying original weights.
- **Flask-based API:** Provides a seamless backend implementation using **Flask** for easy integration.
- **Interactive frontend:** Designed using **HTML/CSS** for a user-friendly experience.

## 🛠️ Technologies Used
- **Programming Language:** Python
- **Machine Learning Framework:** Hugging Face Transformers
- **Model:** EleutherAI/gpt-neo-2.7B (2.7 billion parameters)
- **Optimization Techniques:**
  - **4-bit Quantization (INT4)** to reduce memory footprint
  - **LoRA (Low-Rank Adaptation)** for efficient fine-tuning
- **Web Framework:** Flask (Backend)
- **Frontend Technologies:** HTML, CSS


## 📊 Model Details
### **1. Hugging Face GPT-Neo 2.7B**
The project employs **EleutherAI/gpt-neo-2.7B**, a **Transformer-based LLM**, to generate syntactically and semantically correct code based on user queries.

### **2. Quantization for Optimization**
To enhance computational efficiency, the model undergoes **4-bit Quantization (INT4)**, reducing its size while maintaining accuracy.

### **3. LoRA Fine-Tuning**
LoRA (Low-Rank Adaptation) enables lightweight fine-tuning without modifying original model weights, allowing adaptation for better code generation.

## 🖥️ API Endpoints
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | `/generate_code` | Accepts a text query and returns generated code |
| GET | `/` | Serves the frontend interface |

## 📌 Example Usage
### **Input Query:**
```json
{
  "query": "Write a Python function to find the factorial of a number"
}
```
### **Generated Output:**
```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n-1)
```

## 🏆 Future Enhancements
- Extend support to more programming languages.
- Improve fine-tuning for domain-specific code generation.
- Integrate with cloud-based inference for scalability.




