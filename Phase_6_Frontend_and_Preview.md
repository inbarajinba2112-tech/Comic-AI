# Phase 6 — Frontend & Comic Preview

## Objective
Provide an easy browser interface for entering comic settings and viewing generated panels.

## Frontend Files
```text
templates/index.html
static/style.css
static/script.js
```

## User Workflow
```text
Enter Story
    ↓
Choose Character and Setting
    ↓
Choose Tone and Art Style
    ↓
Choose Number of Panels
    ↓
Generate Comic
    ↓
Story Generation
    ↓
Image Generation
    ↓
Comic Preview
```

## Frontend Responsibilities
- Collect form values
- Send data to the backend
- Show generation status
- Display generated images
- Provide PDF download
- Show errors clearly

## API Workflow
```text
POST /api/generate
       ↓
Story generation
       ↓
Image generation
       ↓
Generated panel files
       ↓
Browser preview
```

## Expected Result
Generated comic panels appear in the Comic Preview section.
