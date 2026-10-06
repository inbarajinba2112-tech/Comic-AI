# Phase 7 — Testing, PDF Export & Error Handling

## Objective
Verify the complete application and produce a downloadable comic PDF.

## PDF Service
```text
services/exporters.py
```

## Testing Checklist
```text
☑ FastAPI starts
☑ Home page loads
☑ Generate API responds
☑ Story is generated
☑ Images are generated
☑ Generated images load
☑ PDF export responds
☑ PDF downloads successfully
```

## Common Errors

### FastAPI Missing
```text
ModuleNotFoundError: No module named 'fastapi'
```
Fix:
```powershell
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

### Uvicorn Cannot Import App
```text
Could not import module "app"
```
Run from the directory containing `app.py`.

### PowerShell Activation Error
```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy RemoteSigned
.\.venv\Scripts\Activate.ps1
```

### JSON Error
If the UI reports:
```text
Unexpected token ... is not valid JSON
```
the AI response may not be clean JSON. Validate/clean the model response before calling `json.loads()`.

### Slow Generation
Use fewer panels, fewer inference steps, or a compatible NVIDIA GPU.

## Expected Result
The complete comic can be generated and exported without blocking errors.
