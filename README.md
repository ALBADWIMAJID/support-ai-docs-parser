<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>support-ai-docs-parser - README</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f9f9f9;
      color: #333;
      margin: 40px;
      line-height: 1.6;
      max-width: 900px;
      margin-left: auto;
      margin-right: auto;
    }
    h1 {
      color: #2c3e50;
    }
    h2 {
      color: #2980b9;
      border-bottom: 1px solid #ddd;
      padding-bottom: 5px;
    }
    code {
      background: #f4f4f4;
      padding: 2px 6px;
      border-radius: 4px;
      font-family: monospace;
    }
    pre {
      background: #f4f4f4;
      padding: 10px;
      border-radius: 6px;
      overflow-x: auto;
    }
    ul {
      padding-left: 20px;
    }
  </style>
</head>
<body>

<h1>🧠 support-ai-docs-parser</h1>

<p><strong>support-ai-docs-parser</strong> is a powerful Python-based tool designed for developers and AI engineers who need to collect, extract, clean, and convert support documentation into multiple formats (HTML, TXT, PDF). This tool is ideal for building AI systems like RAG (Retrieval-Augmented Generation), chatbots, and internal knowledge bases.</p>

<h2>🚀 Features</h2>
<ul>
  <li>🔍 Automatically fetches informative pages from a list of URLs or sitemap.</li>
  <li>🧼 Extracts clean, structured content from messy HTML.</li>
  <li>📄 Saves data in three formats: <code>.html</code>, <code>.txt</code>, and <code>.pdf</code>.</li>
  <li>🌐 Supports Russian, Arabic, English, and any UTF-8 website.</li>
  <li>🧠 Perfect for use with RAG/LLM pipelines.</li>
</ul>

<h2>📁 Output Structure</h2>
<pre>
client_support_output/
├── html/      # Raw and cleaned HTML files
├── text/      # Extracted plain text files
└── pdf/       # Generated PDFs from cleaned HTML
</pre>

<h2>🔧 Installation</h2>
<pre><code>git clone https://github.com/your-username/support-ai-docs-parser.git
cd support-ai-docs-parser

pip install -r requirements.txt

# And install Playwright browser support
pip install playwright
playwright install
</code></pre>

<h2>🛠 Requirements</h2>
<ul>
  <li>Python 3.8+</li>
  <li>requests, beautifulsoup4, lxml</li>
  <li>playwright (for PDF generation)</li>
  <li>pyhtml2pdf (optional fallback)</li>
</ul>

<h2>🧪 How to Use</h2>
<ol>
  <li>Edit <code>app.py</code> and add your list of support URLs or sitemap.</li>
  <li>Run the script:
    <pre><code>python app.py</code></pre>
  </li>
  <li>Check the <code>client_support_output/</code> directory for results.</li>
</ol>

<h2>📦 Use Case Example</h2>
<p>Use this parser to feed high-quality support documentation into:</p>
<ul>
  <li>GPT chatbot using LangChain / Haystack</li>
  <li>Customer service assistant</li>
  <li>FAQ or RAG-based knowledge engine</li>
</ul>

<h2>✍️ Customization</h2>
<ul>
  <li>Change URL language using <code>?hl=ru</code> or <code>?hl=en</code></li>
  <li>Improve accuracy by editing selectors in <code>extract_main_content()</code></li>
  <li>Set <code>max_pages</code> in the script to limit processed pages</li>
</ul>

<h2>📃 License</h2>
<p>MIT License — Free to use and modify for personal and commercial use.</p>

<h2>🙋‍♂️ Author</h2>
<p>Developed with ❤️ by <strong>[Majid Albadwi]</strong>. Contributions welcome!</p>

</body>
</html>
