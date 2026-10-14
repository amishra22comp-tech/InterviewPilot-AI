# InterviewPilot AI

A beginner-friendly mock interview website built with Flask, HTML, CSS, and JavaScript.

## Current features
- Select a target role, interview type, difficulty, and duration
- Predefined practice questions
- Browser text-to-speech for reading questions aloud
- Optional browser speech recognition where supported
- Countdown timer and basic session summary

**Note:** This starter version uses predefined questions. It does not yet connect to an AI provider or save interview history.

## Run on Windows in VS Code

1. Extract the ZIP and open the `InterviewPilot-AI` folder in VS Code.
2. Open Terminal → New Terminal.
3. Create a virtual environment:

   ```powershell
   python -m venv .venv
   ```

4. Activate it:

   ```powershell
   .venv\Scripts\Activate.ps1
   ```

   If PowerShell blocks activation, use `.venv\Scripts\python.exe` for the following commands.

5. Install requirements:

   ```powershell
   pip install -r requirements.txt
   ```

6. Start the app:

   ```powershell
   python app.py
   ```

7. Open `http://127.0.0.1:5000` in Chrome.

Use the Flask URL above rather than opening the HTML file directly. Flask serves the templates and static assets correctly.

## AI API key
No API key is required for the current demo. When real AI evaluation is added, create a local `.env` file from `.env.example` and add your provider key. Do not commit `.env` to GitHub.

## Browser speech support
Speech synthesis and recognition support varies by browser and configuration. If microphone transcription is unavailable, type answers instead.
