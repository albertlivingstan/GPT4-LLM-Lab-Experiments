# GPT4-LLM-Lab-Experiments

A collection of 30 Jupyter Notebook experiments for the Building Applications Using GPT-4 & LLMs lab.

> These practicals use **Ollama + Qwen 2.5 3B** locally. The code does not call the OpenAI GPT-4 API. It demonstrates similar LLM application patterns using a locally hosted model.

## Requirements

- Python 3
- Jupyter Notebook
- Ollama installed
- Model downloaded before going offline: `qwen2.5:3b`

## Setup

1. Install Ollama and download the model while internet is available:
   ```bash
   ollama pull qwen2.5:3b
   ```
2. Start Ollama. On many Mac installations it already runs in the background. If not:
   ```bash
   ollama serve
   ```
   If you see `address already in use`, the Ollama server is probably already running.
3. Check the model:
   ```bash
   ollama list
   ```
4. Install Python dependencies:
   ```bash
   python -m pip install -r requirements.txt
   ```
5. Start Jupyter:
   ```bash
   jupyter notebook
   ```
6. Open any notebook in `experiments/` and run its cells from top to bottom.

## Offline use

Once Ollama and `qwen2.5:3b` are installed locally, the experiments can run without internet. The API address `http://localhost:11434/api/generate` is a local address on the same computer; it is not a public website.

For a college computer with no internet, that computer must already have Ollama and the model installed. A notebook alone cannot provide the model.

## Experiments

01 Grammar Correction Assistant  
02 Sentiment Analysis Application  
03 AI-Based MCQ Generator  
04 AI Study Assistant  
05 AI Flashcard Generator  
06 Meeting Minutes Generator  
07 AI Resume Analyzer  
08 College FAQ Chatbot  
09 Customer Feedback Analyzer  
10 Interview Preparation Assistant  
11 AI Story Generator  
12 Text Translation Assistant  
13 AI Text Summarizer  
14 AI Question Paper Generator  
15 AI Paragraph Rewriter  
16 AI Keyword Extractor  
17 AI Assignment Topic Generator  
18 AI Product Description Generator  
19 AI Daily Task Planner  
20 AI Interview Preparation Assistant  
21 AI Grammar Correction Assistant  
22 Sentiment Analysis Assistant  
23 AI-Based MCQ Generator  
24 AI Study Assistant  
25 AI Flashcard Generator  
26 Meeting Minutes Generator  
27 AI Resume Analyzer  
28 College FAQ Chatbot  
29 Customer Feedback Analyzer  
30 AI Email Assistant  

## Data files

- `data/resume.txt`: Replace the sample text with your own test resume.
- `data/college_faq.txt`: Edit the sample FAQ entries to match your college's verified information.

## Notes

- Run one notebook at a time.
- The first cell in each notebook defines the shared `ask_ollama()` function.
- Generated `.txt` files are saved in the Jupyter working directory.
- Do not put private personal information in sample resumes or test data.
