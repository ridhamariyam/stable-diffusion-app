# Stable Diffusion Application using React with FastAPI

## 1. What is this project about? 

On this project, you can explore how to build a basic React Application using FastAPI as the backend, enabling the generation of images with Stable Diffusion using the Diffusers library from Hugging Face.

### 3.1. What is Stable Diffusion?
It's a deep learning model that generates high-quality images from text prompts. It works using latent diffusion — converting input to a latent space, denoising, and generating visual output.

## Project Structure

```
├── backend                          ----> Contains all the backend FastAPI work
│   ├── dev-requirements.txt
│   ├── main.py                      ----> Endpoints definition
│   ├── requirements.txt
│   ├── run_uvicorn.py
│   ├── schemas.py                   ----> Define your data models here
│   └── services.py                  ----> Define all the heavy load work to be done here.
|                                          in this case all the HuggingFace setup and work for generating the 
|                                          stable diffusion image
└── frontend
    ├── README.md
    ├── package-lock.json
    ├── package.json
    ├── public
    │   ├── index.html
    │   ├── manifest.json
    │   └── robots.txt
    └── src
        ├── App.jsx                 ---> Main App definition where you will embed your components as well
        ├── components
        │   ├── ErrorMessage.jsx
        │   ├── GenImage.jsx        ---> Definition of the UI components as well as the call to the backend 
                                         using fetch API
        │   └── Header.jsx          ---> Minimal Header definition
        └── index.js
```
