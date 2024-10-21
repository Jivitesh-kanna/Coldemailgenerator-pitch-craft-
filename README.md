# Coldemailgenerator-pitch-craft-
# PitchCraft (Cold Mail Generator 📧)

PitchCraft is an AI-powered tool designed to help professionals generate tailored cold emails for job applications or outreach by scraping job posting websites and leveraging large language models (LLMs) to craft the perfect email script. The tool is built using Streamlit, Langchain, ChromaDB, and Groq API for seamless data scraping, storage, and personalized email generation.

## 🚀 Features

Job Posting Scraper: Enter the URL of a job posting, and PitchCraft will automatically scrape the necessary details (such as job title, company name, and job requirements).
AI-Powered Email Generation: Using Langchain and Groq API, PitchCraft creates a customized cold email based on the scraped job posting data.
Persistent Storage: With ChromaDB integrated, the tool stores data efficiently for reuse or future customization.
Simple UI: A clean and interactive Streamlit interface ensures ease of use.

## ✨ Demo
![Screenshot 2024-10-21 204145](https://github.com/user-attachments/assets/7b4e6638-0874-4671-a116-f31f160177f3)
![Screenshot 2024-10-21 204239](https://github.com/user-attachments/assets/1ca4b477-55b7-4cbf-8be9-8bb89d6c0087)
![Screenshot 2024-10-21 204259](https://github.com/user-attachments/assets/20d6cfed-4cbc-4de8-a391-8ab2e6c5b45a)


## 🛠️ Technologies Used

 Streamlit: For building an interactive and intuitive front-end user interface.
 Langchain: To handle natural language processing and LLM integration for crafting personalized emails.
 Groq API: Utilized for processing large datasets and ensuring efficient query generation.
 ChromaDB: For vector storage and persistent data management, ensuring data scalability and fast query performance.
 BeautifulSoup (bs4): For scraping job posting content from websites.
  
## 📂 Project Structure

```
📁 PitchCraft/
├── 📁 app/
│   ├── chains.py              # Handles the scraping and email generation logic
│   ├── portfolio.py           # Portfolio class to manage job data
│   ├── utils.py               # Utility functions (e.g., text cleaning)
│   └── main.py                # Streamlit app execution script
├── 📁 resource/
│   └── my_portfolio.csv       # CSV containing predefined tech stacks and links
├── .env                       # Environment variables including API keys
├── README.md                  # Project README file
├── requirements.txt           # Python package dependencies
└── .streamlit/                # Streamlit configuration files
```

## ⚙️ Installation

1.Clone the Repository:

    ```bash
    git clone https://github.com/your-username/PitchCraft.git
    cd PitchCraft
    ```

2.Set Up the Virtual Environment:

    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows: .venv\Scripts\activate
    ```

3.Install Dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4.Set Up Environment Variables:

    Create a `.env` file in the root directory and add your Groq API Key and other necessary environment variables:

    ```bash
    GROQ_API_KEY=<your-groq-api-key>
    ```

5.Run the Streamlit App:

    ```bash
    streamlit run app/main.py
    ```

6.Navigate to your local server: 
   The app will run on `http://localhost:8501/` by default.

## 📊 Usage

1. Open the Streamlit app in your browser.
2. Enter the URL of a job posting.
3. The app scrapes the job description and uses AI to generate a cold email tailored to the job.
4. The email draft can be modified or saved for future reference.

## 🐛 Troubleshooting

- File Not Found Errors: Ensure that the file `app/resource/my_portfolio.csv` exists or modify the file path in `portfolio.py`.
- Missing Packages**: Ensure all necessary dependencies are installed via `pip install -r requirements.txt`.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-username/PitchCraft/issues).

1. Fork this repository.
2. Create your feature branch: `git checkout -b my-new-feature`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin my-new-feature`.
5. Submit a pull request.



