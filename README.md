Here’s the entire README.md file, fully formatted and ready for you to copy:

Colab Web Crawler

This repository contains a Google Colab-based Web Crawler with an interactive user interface that simplifies crawling and extracting text from websites. The tool recursively visits all pages within the same domain, collects their text content, and saves it as .txt files in a Google Drive folder.

Features
	•	Interactive UI: Built with ipywidgets, featuring buttons and text fields for easy input and control.
	•	Google Drive Integration: Saves crawled text directly into a specified folder in your Drive.
	•	Text Extraction: Captures and stores the title, URL, timestamp, and full text of each page.
	•	Recursive Crawling: Automatically follows links within the same domain.
	•	Unique Filenames: Ensures no duplicates by appending timestamps to file names.

How It Works
	1.	Mount Google Drive: Store crawled data directly in your Drive.
	2.	Specify a Folder: Create or verify a folder for saving the results.
	3.	Enter a URL: Provide the starting URL to crawl.
	4.	Start Crawling: The script recursively gathers text from all pages on the same domain and saves them as .txt files.

Setup and Usage

1. Clone the Repository

Clone this repo to access the notebook:

git clone https://github.com/YOUR-USERNAME/colab-web-crawler.git
cd colab-web-crawler

2. Open the Notebook in Google Colab
	1.	Visit Google Colab.
	2.	Click “File” → “Upload Notebook” (or open the .ipynb file directly from your GitHub).
	3.	Upload the file colab_web_crawler.ipynb.

3. Install Dependencies

If running locally (not in Colab), install required Python packages:

pip install -r requirements.txt

4. Run the Notebook
	1.	Mount Google Drive to store results.
	2.	Specify the folder name for saving .txt files.
	3.	Enter the starting URL of the website you want to crawl.
	4.	Click “Crawl & Save” to begin. The extracted text is saved in the specified Drive folder.

Output

Each .txt file contains:
	•	Title: The page’s title or a default value.
	•	URL: The full URL of the crawled page.
	•	Timestamp: The date and time of crawling.
	•	Text Content: The full extracted text.

File names follow this pattern:

PageTitle_Timestamp.txt

Example Use Cases
	•	Data Extraction: Collect text data for analysis or research.
	•	Web Archiving: Save textual content from websites for offline use.
	•	Content Review: Extract and inspect website content easily.

Notes
	•	Respect Terms of Service: Always check the website’s robots.txt and Terms of Service before crawling.
	•	Politeness: The crawler uses a 1-second delay between requests. Adjust as needed to avoid overloading servers.
	•	Limits: For large sites, set a page limit (max_pages) to avoid excessive crawling.

Requirements
	•	Python 3.6+
	•	Google Colab or Jupyter Notebook
	•	Libraries: requests, beautifulsoup4, ipywidgets

Install dependencies via:

pip install -r requirements.txt

License

This project is licensed under the MIT License.

Contributing

Feel free to fork the repository, submit issues, or open pull requests to improve the tool. Contributions are welcome!

Contact

For questions or suggestions, please contact thomas.f@febus.ai
