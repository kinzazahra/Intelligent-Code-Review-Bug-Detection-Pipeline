# AI Code Review Pipeline

---

### Overview

This project demonstrates a simple AI-powered code review pipeline that analyzes Python code for common quality issues, generates feedback, calculates a quality score, suggests improvements, and visualizes the results.

---

### Features

- Automated code quality checks
- Detection of missing type hints
- Detection of missing docstrings
- Basic division-by-zero safety validation
- Code quality scoring system
- Suggested improved code output
- Quality score visualization using Matplotlib

---

### Project Workflow

1. Load required libraries.
2. Provide sample Python code.
3. Run automated review checks.
4. Generate a list of detected issues.
5. Calculate a code quality score.
6. Produce an improved version of the code.
7. Visualize the final quality score.

---

### Technologies Used

- Python
- Pandas
- Matplotlib
- Regular Expressions (re)

---

### Example Issues Detected

- Missing type hints
- Missing docstrings
- Potential division-by-zero risk

---

### Quality Score Formula

```python
score = 100 - len(issues) * 15
Sample Input
def divide(a,b):
    return a/b
Suggested Improved Code
def divide(a: int, b: int) -> float:
    """Safely divide two numbers"""

    if b == 0:
        raise ValueError("Division by zero")

    return a / b
Visualization

The project generates a bar chart displaying the overall code quality score.

Installation
pip install transformers pandas matplotlib
Run the Notebook
jupyter notebook ai_code_review_pipeline.ipynb
Future Improvements
Integration with LLMs for advanced code reviews
Support for multiple programming languages
CI/CD integration
GitHub Pull Request review automation
Security vulnerability detection
Complexity and performance analysis
Project Structure
.
├── ai_code_review_pipeline.ipynb
└── README.md

```

---

### Author

**Kinza Zahra**
