# Gemini RAG Implementation

This repository contains an implementation of a Retrieval Augmented Generation (RAG) system, developed as part of an astronomy research project. The goal is to facilitate the exploration and summarization of multimodal data related to the Apollo 11 mission.

## Overview

This project allows users to search and summarize information from various data sources about the Apollo 11 mission, using a RAG system. The data includes:

- **Text:** Selected pages from NASA's final post-mission report.
- **Video:** Clips of Neil Armstrong and Buzz Aldrin's moonwalk and flag-raising.
- **Audio:** Highlights of the communication between astronauts and mission control.

## Features

- **Optical Character Recognition (OCR):** Extracts text from images of the report pages.
- **Video Analysis:** Processes and retrieves relevant clips.
- **Audio Processing:** Extracts and analyzes communication highlights.
- **RAG System:** Combines retrieval and generation to provide comprehensive responses to user queries.

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/Gemini-RAG.git
    cd Gemini-RAG
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Set up environment:**
    - Ensure you have the necessary API keys and credentials set up for accessing Google Cloud and other services.

## Usage

1. **Run the Jupyter Notebook:**
    Open `RAG_implementation_Gemini.ipynb` in Jupyter Notebook or Jupyter Lab.

2. **Configure API Key:**
    Ensure you have your Google API key set up:
    ```python
    from google.colab import userdata
    GOOGLE_API_KEY = userdata.get('GOOGLE_API_KEY')
    genai.configure(api_key=GOOGLE_API_KEY)
    ```

3. **Execute the notebook:**
    Follow the instructions provided in the notebook cells to process and analyze the data.


## Acknowledgements

- NASA for providing the Apollo 11 mission data.
- The developers and maintainers of the libraries and tools used in this project.

