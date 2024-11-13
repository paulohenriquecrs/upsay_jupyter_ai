# UPSayAI: Generative AI Toolkit for Jupyter Notebooks

**UPSayAI** is a Python toolkit developed for students at Université Paris-Saclay, designed to integrate Generative AI features directly into Jupyter Notebooks. Created during an M1 internship with the GALaC team at [LISN](https://www.lisn.fr), this toolkit aims to enhance the educational experience in STEM courses by providing an interactive AI-powered environment for practical learning, coding, and analysis.

## Overview

In an academic setting, particularly within STEM fields, Jupyter Notebooks have become a core tool for teaching and learning. Professors often prepare notebooks that combine theoretical explanations with coding exercises, allowing students to practice by completing, modifying, or creating code. The UPSayAI toolkit enriches this environment by integrating a Retrieval-Augmented Generation (RAG) system, making course-specific information accessible within prompts. This allows students to interact with Generative AI for help with code suggestions, explanations, and more.

## Key Features

- **Flexible Configuration**: Initialize UPSayAI as an object with customizable parameters for flexibility in experimentation and testing.
- **RAG-Enhanced Prompts**: Employs a Retrieval-Augmented Generation (RAG) system to enrich AI-generated responses with relevant course materials.
- **Custom Magic Commands**: Includes specialized magic commands to streamline Generative AI interactions within Jupyter Notebooks.
- **Educational Focus**: Designed with the unique needs of STEM students and educators in mind, offering a seamless way to access AI support while working on coding and analysis tasks.

## Getting Started

To start using UPSayAI in your Jupyter environment, install the `upsay_jupyter_ai` package, then initialize an instance of the `UPSayAI` class with your preferred settings. 

### Installation

```bash
pip install upsay_jupyter_ai
```

### Usage

```python
from upsay_jupyter_ai import UPSayAI

UPSayAI(model_name="aristote/llama",
        model_access_token=my_access_token,
        model_temperature=0.8,
        model_max_tokens=2048,
        rag_model="dpr",
        rag_min_relevance=0.5,
        rag_max_results=5,
        recommendation_min_relevance=0.7,
        quiz_difficulty="moyen",
        quiz_min_relevance=0.2,
        quiz_max_results=100,
        num_questions_quiz=5,
        course_corpus_file="corpus_ISD.csv");

# Start using AI-enhanced magic commands within your Jupyter Notebook
```

## Motivation

UPSayAI was inspired by the need for a reliable, open-source Generative AI tool within the educational environment of Université Paris-Saclay. Developed to empower students, the toolkit serves as an assistant that guides them through complex coding tasks and enriches their learning experience by providing interactive AI support in a familiar setting.

## License

This project is licensed under the MIT License. See the [PyPI](https://pypi.org/project/upsay_jupyter_ai) for details.

