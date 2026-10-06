# Phase 3 — FastAPI Backend

## Objective
Create the backend server that connects the web interface with ComicCraft services.

## Main File
```text
app.py
```

## Run the Application
From the folder containing `app.py`:
```powershell
python -m uvicorn app:app --reload
```

## Browser
```text
http://127.0.0.1:8000
```

## Successful Startup
```text
INFO: Uvicorn running on http://127.0.0.1:8000
INFO: Application startup complete.
```

## Backend Responsibilities
- Serve the web page
- Receive generation requests
- Call the story generator
- Call the image generator
- Serve generated images
- Provide PDF export

## Common Error
If you see:
```text
Could not import module "app"
```
run Uvicorn from the directory containing `app.py`.

## Expected Result
The ComicCraft website opens successfully in the browser.
