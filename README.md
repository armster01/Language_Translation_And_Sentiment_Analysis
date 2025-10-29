# 🌐 Language Translation & Sentiment Analysis

A powerful Streamlit-based web application that leverages Google's Gemini AI to provide seamless language translation, sentiment analysis, and visual word cloud generation. Translate text between multiple languages while analyzing emotional tone and generating insightful visualizations.

## 📋 Features

- **Multi-Language Translation**: Support for 13+ languages including English, Spanish, French, German, Italian, Portuguese, Dutch, Russian, Japanese, Korean, Chinese, Arabic, and Hindi
- **Real-time Sentiment Analysis**: Analyze sentiment of both original and translated text with confidence scores and detailed explanations
- **Interactive Word Clouds**: Generate visual word clouds for original and translated text to highlight key terms
- **Flexible Input Methods**: Type text directly or upload text files for processing
- **Modern UI**: Clean, responsive interface built with Streamlit and Plotly for an intuitive user experience
- **AI-Powered**: Utilizes Google's Gemini Pro model for accurate translations and sentiment analysis

## 🚀 Installation

### Prerequisites

- Python 3.8 or higher
- A Google Gemini API key (obtain from [Google AI Studio](https://makersuite.google.com/app/apikey))

### Setup

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd lang_tran
   ```

2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv venv
   venv\Scripts\activate  # On Windows
   # or
   source venv/bin/activate  # On macOS/Linux
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**
   - Create a `.env` file in the root directory
   - Add your Gemini API key:
     ```
     GEMINI_API_KEY=your_api_key_here
     ```

## 🎯 Usage

1. **Run the application:**
   ```bash
   streamlit run app.py
   ```

2. **Access the app:**
   - Open your browser and navigate to `http://localhost:8501`

3. **Using the app:**
   - Choose your input method (type text or upload a file)
   - Select source and target languages
   - Click "Translate" to process your text
   - View translation, sentiment analysis, and word clouds

## ⚙️ Configuration

The application uses the following configuration options (defined in `config.py`):

- **Page Settings**: Title, icon, and layout
- **API Settings**: Model name, temperature, max tokens
- **Supported Languages**: Dictionary of language codes and names

You can modify these settings by editing the `Config` class in `config.py`.

## 📦 Dependencies

- `streamlit==1.29.0` - Web app framework
- `python-dotenv==1.0.0` - Environment variable management
- `google-generativeai==0.3.1` - Google Gemini API client
- `wordcloud==1.9.2` - Word cloud generation
- `pandas==2.1.4` - Data manipulation
- `matplotlib==3.8.2` - Plotting library
- `plotly==5.18.0` - Interactive charts

## 🏗️ Project Structure

```
lang_tran/
├── app.py              # Main Streamlit application
├── config.py           # Configuration settings
├── utils.py            # Utility functions (translation, sentiment, word clouds)
├── components.py       # Reusable UI components
├── requirements.txt    # Python dependencies
├── .gitignore         # Git ignore rules
├── README.md          # Project documentation
└── .env               # Environment variables (not in repo)
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Powered by [Google Gemini AI](https://ai.google.dev/)
- Word clouds generated using [WordCloud](https://github.com/amueller/word_cloud)
- Charts created with [Plotly](https://plotly.com/)

## 📞 Support

If you encounter any issues or have questions, please open an issue on the GitHub repository.

---

**Note:** Make sure to keep your `.env` file secure and never commit API keys to version control.