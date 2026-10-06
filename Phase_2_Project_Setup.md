# Phase 2 — Project Structure & Environment Setup

## Objective
Create the ComicCraft project structure and prepare the Python development environment.

## Project Structure
```text
ComicCraft/
├── app.py
├── requirements.txt
├── README.md
├── services/
│   ├── story_generator.py
│   ├── image_generator.py
│   └── exporters.py
├── templates/
│   └── index.html
├── static/
│   ├── script.js
│   └── style.css
└── generated/
```

## Create Virtual Environment
```powershell
python -m venv .venv
```

## Activate
```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy RemoteSigned
.\.venv\Scripts\Activate.ps1
```

## Install Dependencies
```powershell
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## GitHub Safety
Do not upload:
```text
.venv/
__pycache__/
.env
API keys
large AI model/cache files
```

## Expected Result
The project has a clean structure and an isolated Python environment.
