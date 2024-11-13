# Background Swap Web App

A web app to swap the background of an image using Stable Diffusion and SAM (Segment Anything Model).

## Features
- Segment subjects using SAM.
- Replace backgrounds with Stable Diffusion.
- Easy-to-use Gradio interface.

## Installation
Install dependencies with:
```
pip install -r requirements.txt
```

## Usage
Run the app with:
```
python background_swap_ai_app.py
```
Upload an image, enter a prompt, and generate a new background.

## Dependencies
- `Pillow`, `requests`, `transformers`, `diffusers`, `torch`, `gradio`, `numpy`

