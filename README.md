# 🧠 support-ai-docs-parser

A Python-based utility for extracting clean, informative content from support/documentation websites and exporting it into structured formats (HTML, TXT, PDF). Ideal for RAG-based AI systems, LLM chatbots, and internal knowledge tools.

---

## 🚀 Features

- 🔍 Automatically scrapes a list of URLs or sitemap.xml.
- 🧼 Extracts the main informative content only (filters ads, menus, etc.).
- 📄 Converts content into:
  - Cleaned HTML (`/html`)
  - Plain text (`/text`)
  - PDF format (`/pdf`)
- ⚙️ Smart content detection (word/link ratio, main containers like `<main>`, `<article>`).
- 🌍 Supports multilingual content (e.g., Arabic, English, Russian).
- 📥 Works with any public support website (e.g., Google, Microsoft, Yandex Help).

---

## 📁 Output Structure


---client_support_output/ ├── html/ # Cleaned HTML content ├── text/ # Extracted plain text └── pdf/ # Converted PDF documents

yaml
Copy
Edit


## 📦 Installation

```bash
git clone https://github.com/your-username/support-ai-docs-parser.git
cd support-ai-docs-parser

# Install Python dependencies
pip install -r requirements.txt

# Install Playwright browser driver
pip install playwright
playwright install
🧪 Usage
Add your list of URLs (or sitemap) inside app.py in all_website_urls.
all_website_urls = [
  "https://support.google.com/accounts/answer/27441?hl=ru",
  "https://support.google.com/accounts/answer/6010255?hl=ru",
  ...
]

Run the script:
python app.py
🧠 Use Case
This tool is ideal if you're building:

✅ A retrieval-augmented generation (RAG) system.

🤖 A chatbot based on documentation pages.

🧾 A knowledge base using real-time support articles.

🔄 Automatic documentation syncing.

⚙️ Configuration
You can limit the number of processed pages with:
process_urls_from_sitemap(all_website_urls, max_pages=5)

👨‍💻 Author
Developed by [Majid Albadwi], 2025.
Contributions, forks, and issues are welcome!

