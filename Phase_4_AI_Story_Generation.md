# Phase 4 — AI Story Generation

## Objective
Generate a structured comic story from the user's idea.

## Service
```text
services/story_generator.py
```

## Inputs
```text
Story Prompt
Main Character
Setting
Tone
Art Style
Number of Panels
```

## Example
```text
Story:
A young explorer named Maya discovers a mysterious glowing door
inside an enchanted forest. Behind it is a magical world that
needs her help. She must overcome her fear and save the forest.

Character: Maya
Setting: Enchanted Forest
Tone: Dramatic
Art Style: Comic Book
Panels: 2
```

## Expected Panel Data
```json
{
  "title": "The Mysterious Door",
  "narration": "Maya enters the enchanted forest.",
  "dialogue": "What is behind this door?",
  "image_prompt": "A young explorer standing before a glowing magical door"
}
```

## Fallback
ComicCraft includes fallback story logic so the application can continue when an external AI service is unavailable.

## Expected Result
The story is converted into structured panel information ready for image generation.
