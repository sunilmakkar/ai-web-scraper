# AI Web Scraper

## Overview

This is an AI-powered web scraping application built with Streamlit, Selenium, and Ollama, allowing users to scrape website content and extract specific information using natural language prompts.

## Features

- 🌐 Web Scraping: Extract content from any website
- 🤖 AI-Powered Parsing: Use natural language to extract precise information
- 🖥️ User-Friendly Interface: Simple Streamlit web application
- 🔍 CAPTCHA Handling: Integrated CAPTCHA solving mechanism

## Prerequisites

- Python 3.10+
- Anaconda or Miniconda
- Ollama (with Mistral model)
- Chrome WebDriver

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/sunilmakkar/ai-web-scraper.git
cd ai-web-scraper
```

### 2. Create Conda Environment

```bash
conda env create -f environment.yaml
conda activate ai_web_scraper_env
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Ollama

Ensure Ollama is installed and the Mistral model is available:

```bash
ollama pull mistral
```

### 5. Configure Bright Data Proxy (Optional)

Replace the `SBR_WEBDRIVER` in `scrape.py` with your Bright Data credentials.

## Usage

Run the Streamlit application:

```bash
streamlit run main.py
```

### How to Use

1. Enter a website URL
2. Click "Scrape Site" to extract content
3. Describe what information you want to parse
4. Click "Parse Content" to extract specific details

## Dependencies

- Streamlit
- Selenium
- BeautifulSoup
- Langchain
- Ollama
- Mistral LLM

## Limitations

- Requires Bright Data proxy for advanced scraping
- CAPTCHA solving may not work for all websites
- Parsing accuracy depends on the Mistral model's performance

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Future Improvements

While the current implementation provides a versatile web scraping solution, the most significant enhancement would be to specialize the scraper for a specific industry or use case. By tailoring the scraper to solve a niche problem, such as automated competitive analysis for e-commerce, real estate market research, or job market intelligence, the tool could provide more targeted and valuable insights. Personalization would involve creating custom parsing logic, industry-specific data extraction rules, and potentially integrating domain-specific AI models to improve accuracy and relevance of extracted information.

## License

MIT License

## Acknowledgements

- Inspired by Tech With Tim's tutorial
- Powered by Ollama and Mistral LLM
