# FinGenius App

[Website](https://fingenius.app) | [Twitter](https://x.com/FinGeniusAPP)

## Open-Source AI-Powered Personalized Finance Assistant

FinGenius is an **AI-powered personal finance assistant** that helps users **analyze, optimize, and automate** their financial activities. Using **machine learning** and **real-time data analytics**, FinGenius offers:
- **Personalized financial insights**
- **Smart investment strategies**
- **Risk management solutions**

---

## Setup

### Option 1: Jupyter Notebook
1. Use the notebook `notebook/01_financial-analysis-notebook.ipynb` to set up your project and generate the data.
2. Use the notebook `notebook/02_gradio-gpt.ipynb` to test the advisor interface.

### Option 2: Python Script
1. Clone the repository:
   ```sh
   git clone https://github.com/FinGeniusAPP/FinGeniusAPP.git
   cd FinGeniusAPP
   ```
2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Copy example environment file and update values:
   ```sh
   cp example.env .env
   ```
4. Update the `.env` file with the following:
   - **`OPENAI_API_KEY`**: Your OpenAI API key
   - **`GOOGLE_APPLICATION_CREDENTIALS`**: Path to your Google Cloud credentials JSON file (if using Google Sheets)
   - **`USE_GOOGLE_SHEETS`**: Set to `true` if using Google Sheets, `false` if using local CSV
   - **`DUMMY_DATA_SPREADSHEET`**: URL of the dummy data Google Sheet (provided in `example.env`)

---

## Data
The dataset is a CSV file with the following structure:
- **Date**: Transaction date
- **Description**: Description of the transaction
- **Amount**: Transaction amount
- **Category**: Transaction category

This synthetic data was generated using OpenAI's GPT-4 Preview model.

---

## Usage
### Running the Main Application (Python Script)
```sh
python main.py
```

---

## Contributing
FinGenius is an **open-source** project, and contributions are welcome! You can:
- Report issues
- Submit pull requests
- Suggest improvements

For more details, check the [GitHub repository](https://github.com/FinGeniusAPP/FinGeniusAPP).

---

## License
This project is licensed under the **MIT License**.

