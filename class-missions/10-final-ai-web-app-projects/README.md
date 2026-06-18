# Unit 7: Final AI Web App Projects

There are two final project levels.

## Core Final Project: House Price Prediction Web App

This is the main project students are expected to understand deeply.

Students build:

- React frontend form
- FastAPI backend
- trained regression model
- prediction result display
- testing table
- README
- reflection
- AI use log

Students must be able to explain:

- What the user inputs are
- What the model predicts
- How React sends data to FastAPI
- How FastAPI returns the prediction
- What the model limitations are
- What student-written logic they wrote, such as input validation, result interpretation, or testing function

## Showcase Project: MNIST Digit Recognition Web App

This can be used as an impressive AI showcase.

The teacher may pre-write the complex image-processing scaffold:

- canvas drawing
- image upload
- image resizing
- grayscale conversion
- normalization
- model input shape conversion
- frontend image preprocessing
- model loading
- prediction endpoint structure

Students should still understand the pipeline:

```text
drawing or uploaded image
→ preprocessing
→ 28x28 grayscale input
→ normalized model input
→ model prediction
→ JSON response
→ frontend result display
```

Students are responsible for React UI, backend call, prediction display, confidence/top result if available, testing several digits, README, reflection, and explaining where the model fails.

Do not require students to write the full image preprocessing pipeline from scratch.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
