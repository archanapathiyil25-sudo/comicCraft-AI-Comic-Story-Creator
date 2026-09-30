# ComicCraft - AI Comic Story Creator using Gemini Models

## 1. Project Overview
ComicCraft is a web application that uses Google's Gemini API to transform a user's simple story idea into a structured comic storyboard. The generated comic contains a title, logline, characters, multiple panels, narration, dialogue, an ending and a moral.

## 2. Main Features
- User-friendly Streamlit interface
- Story idea and genre selection
- Configurable number of comic panels
- AI-generated characters and story flow
- Structured JSON output from Gemini
- Panel-by-panel storyboard display
- Download generated comic as JSON
- Download a standalone HTML comic storyboard

## 3. Technology Stack
- Python
- Streamlit
- Google Gemini API / Google GenAI SDK
- Pydantic structured output
- HTML/CSS

## 4. Architecture
User Input -> Streamlit UI -> Prompt Builder -> Gemini Model -> Structured JSON -> Pydantic Validation -> Comic Storyboard -> JSON/HTML Download

## 5. Setup
### Step 1: Install Python
Use Python 3.10 or newer.

### Step 2: Install packages
```bash
pip install -r requirements.txt
```

### Step 3: Create a Gemini API key
Create an API key using Google's Gemini API / AI Studio account and keep it private.

### Step 4: Set the API key
Windows PowerShell:
```powershell
$env:GEMINI_API_KEY="YOUR_KEY"
```

Linux/macOS:
```bash
export GEMINI_API_KEY="YOUR_KEY"
```

Or copy `.env.example` to `.env` and configure it with the environment method used by your deployment. Never upload a real API key to GitHub.

### Step 5: Run
```bash
streamlit run app/app.py
```

## 6. Demo Example
Story idea: "A shy student discovers a tiny robot that can repair broken things."

Expected output:
- Catchy comic title
- Character list
- 3-10 connected panels
- Scene descriptions
- Narration
- Dialogue
- Ending
- Moral

## 7. Important Security Rule
Do NOT place a real Gemini API key inside `app.py` or upload it to GitHub. Use an environment variable or a deployment secret.

## 8. Project Scope
This version creates a comic storyboard using Gemini-generated text and panel descriptions. It does not claim to generate finished comic artwork.
