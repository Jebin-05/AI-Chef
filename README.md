# 🍽️ AI-Chef: Intelligent Food Analyzer

AI-Chef is an AI-powered food analysis application that uses advanced vision-language models to provide comprehensive culinary insights. Upload any food image and instantaneously get ingredient lists, step-by-step recipes, nutritional breakdowns, and more.

## Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Jebin-05/AI-Chef.git
   cd AI-Chef
   ```
2. Create and activate a Python virtual environment (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. (Optional) Configure the Gemini API key:
   - Create a `.env` file in the project root with:
     ```
     GEMINI_API_KEY=your_actual_api_key_here
     ```
   - Get your key from https://makersuite.google.com/app/apikey

## Usage

Run the Streamlit application of your choice:

- Main application:
  ```bash
  streamlit run app.py
  ```
- Cloud-based Gemini interface:
  ```bash
  streamlit run gemini.py
  ```

Open your browser at `http://localhost:8501` and follow these steps:
1. Click **Upload Image** to select a food photo.
2. Choose an analysis mode:
   - **Get Ingredients:** Lists ingredients with quantities.
   - **Get Recipe:** Generates cooking instructions.
   - **Get Calories:** Shows nutritional analysis.
   - **Ask Questions:** Enter any custom question.
3. View detailed AI-driven results instantly.
