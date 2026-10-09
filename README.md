# Prompt_Engineering
```text
Explain Artificial Intelligence.
```

## 2. One-shot Prompting

One-shot prompting provides the model with one example to guide its response.

### Example

```text
Example:
Question: What is Python?
Answer: Python is a programming language.

Question: What is Java?
Answer:
```

## 3. Few-shot Prompting

Few-shot prompting provides multiple examples to help the model understand the expected response format.

### Example

```text
Example 1:
Input: I love this product.
Sentiment: Positive

Example 2:
Input: This product is terrible.
Sentiment: Negative

Input: The product is amazing.
Sentiment:
```

## 4. Chain-of-Thought (CoT) Prompting

Chain-of-Thought prompting encourages the model to break down a problem into intermediate steps before producing an answer.

### Example

```text
Solve this problem step by step:

A student has 5 books and buys 3 more.
How many books does the student have now?
```

## 5. Manual Chain-of-Thought Prompting

Manual Chain-of-Thought prompting provides predefined steps or a structured approach for the model to follow.

### Example

```text
Solve the problem using these steps:

1. Identify the given information.
2. Determine the operation required.
3. Perform the calculation.
4. Provide the final answer.

Problem: A student has 10 apples and gives away 4.
How many apples remain?
```

## 6. Tree-of-Thought (ToT) Prompting

Tree-of-Thought prompting explores multiple possible approaches to a problem and compares them to identify a suitable solution.

### Example

```text
Suggest three different ways to reduce plastic pollution.
Evaluate the advantages and disadvantages of each approach.
Recommend the most practical solution.
```

---

## ⚙️ LLM Configuration

The application allows users to experiment with different language model settings.

* **Temperature:** Controls the randomness of generated responses. Lower values generally produce more predictable outputs, while higher values encourage greater variation.
* **Maximum Tokens:** Sets the maximum number of tokens the model can generate in a response.

The actual output also depends on the model, prompt, and other generation settings.

---

## 🛠️ Technologies Used

* **Python** – Application logic
* **Streamlit** – Interactive user interface
* **Hugging Face Transformers** – Language model integration
* **SmolLM2** – Local language model for response generation
* **PyTorch** – Model inference backend

---

## 📁 Project Structure

```text
Prompt-Engineering-App/
│
├── app.py
├── requirements.txt
└── README.md
```

*Note: The filenames above assume your main application file is named `app.py`.*

---

## 💻 Installation and Setup

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
cd Prompt-Engineering-App
```

### 2. Create a Virtual Environment (Optional)

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run app.py --server.port 8502
```

Open the local application in your browser:

http://localhost:8502

**Note:** The first run may take longer because the Hugging Face model may need to be downloaded. Downloading requires an internet connection unless the model is already cached locally.

---

## 📦 Requirements

Create a `requirements.txt` file containing the dependencies used by your application:

```text
streamlit
transformers
torch
```

Install them using:

```bash
pip install -r requirements.txt
```

---

## 🌟 Key Features

* Interactive interface for testing prompts.
* Six prompting techniques in one application.
* Local language model inference.
* Adjustable temperature and maximum token settings.
* Real-time response generation.
* Hands-on experimentation with prompt design.

---

## 🎓 Learning Outcomes

Through this project, I learned how to:

* Understand and implement different prompt engineering techniques.
* Integrate a Hugging Face language model into a Streamlit application.
* Experiment with prompt structures and generation parameters.
* Build an interactive AI application using Python.
* Explore how prompting strategies influence LLM outputs.

---

## 👩‍💻 Author

**D. Hasini**

B.Sc. Computer Science with Artificial Intelligence

```

**Before uploading to GitHub:** Check that your model name, Python filename, and dependencies match your actual code. Also, the local Streamlit URL will not work for other users unless they run the application on their own computers.
```
