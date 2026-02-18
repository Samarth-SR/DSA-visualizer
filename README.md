# DSA Visualizer

A Python-based application that visualizes Data Structures and Algorithms using Manim and Gemini AI.

## Prerequisites

To run this application, you need:

1.  **Python 3.10+** installed.
2.  **FFmpeg** installed and added to your system PATH.
    *   *Windows*: `winget install Gyan.FFmpeg`
    *   *Mac*: `brew install ffmpeg`
    *   *Linux*: `sudo apt install ffmpeg`
3.  **Manim** dependencies (optional but recommended for text rendering: LaTeX/MikTeX).

## Installation

1.  Unzip this folder.
2.  Open a terminal/command prompt in this folder.
3.  Install Python dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  Run the application:
    ```bash
    streamlit run app.py
    ```
    *(Or double-click `run.bat` on Windows if configured)*

2.  The app will open in your browser.
3.  Enter your Gemini API Key in the sidebar.
4.  Paste your DSA code and click "Visualize".

## Configuration

*   **API Key**: You can store your API key in a `.env` file or `secrets.toml` if you prefer, but the UI allows manual entry.
*   **Models**: The app automatically selects the best available Gemini model (`flash`, `pro`) for your account.

## Troubleshooting

*   **Animation Error**: If animations fail, ensure FFmpeg is correctly installed and accessible from the terminal (`ffmpeg -version`).
*   **Rate Limits**: The app handles rate limits automatically by switching models. If it persists, wait a minute.
