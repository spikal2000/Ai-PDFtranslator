# Ai-PDFtranslator
 
## Translate PDFs to Any Language with OpenAI

Ai-PDFtranslator is a lightweight Python tool that extracts text from PDF documents and translates it to any language using OpenAI's powerful language models. Perfect for researchers, students, and professionals who need to quickly understand documents in foreign languages.



### Features

- **Simple Interface**: Interactive prompts make translation easy without complex commands
- **Support for Any Language**: Translate to English or any other language supported by OpenAI
- **Formatting Preservation**: Maintains document structure during translation
- **Chunk Processing**: Handles large documents by processing text in manageable chunks
- **Progress Tracking**: Shows real-time progress during translation


### Requirements

- Python 3.6+
- OpenAI API key
- Required packages: `openai`, `PyPDF2`

### Installation

```bash
# Clone the repository
git clone https://github.com/spikal2000/Ai-PDFtranslator.git
cd pdflingo

# Install dependencies
pip install openai PyPDF2
```

### Usage

Simply run the script and follow the interactive prompts:

   Run the Translator_Ai.ipynb 


The script will ask for:
1. Your OpenAI API key (or use the OPENAI_API_KEY environment variable)
2. Path to the PDF file
3. Target language (defaults to English)
4. Output file path (optional)


### Example

```
Enter your OpenAI API key: sk-...
Enter the path to your PDF file: German-paper.pdf
Enter target language (press Enter for English): English
Enter output file path (press Enter for default): 

Extracting text from research_paper_spanish.pdf...
Translating 3 chunks...
Translating chunk 1/3...
Translating chunk 2/3...
Translating chunk 3/3...
Translation completed and saved to german_paper_translated_to_English.txt
```

### How It Works

1. **Text Extraction**: Uses PyPDF2 to extract text content from PDF files
2. **Chunking**: Splits large documents into manageable pieces to avoid API token limits
3. **Translation**: Sends each chunk to OpenAI's API for high-quality translation
4. **Output**: Saves the translated text to a file, preserving the original formatting


