-----

# Indeed Job Scraper with Apify 🤖

This project automates scraping job postings from **Indeed** using the **Apify Indeed Scraper**. It extracts key details, cleans the job description, and saves the data into a structured **CSV file** ready for analysis.

-----

## ✨ Key Features

  - ✅ **Automated Scraping**: Fetches job postings from Indeed based on your search query.
  - 🧹 **Data Cleaning**: Automatically removes HTML tags from job descriptions for clean, readable text.
  - 📄 **Structured Output**: Saves all extracted data into a well-organized `.csv` file.
  - 🔐 **Secure**: Keeps your API keys safe and out of the codebase using a `.env` file.

-----

## 📂 Project Structure

```
.
├── job_scraper.py      # Main Python script for the scraper
├── .env                # Stores APIFY_TOKEN and ACTOR_ID (kept private)
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

-----

## 🚀 Getting Started

### Prerequisites

  - Python 3.x
  - An [Apify account](https://apify.com/) (a free account with credits is available)

### 🛠️ Installation & Setup

1.  **Clone the Repository**

    ```bash
    git clone https://github.com/Karthih2/Cybernaut-Project-Indeed-Web-Scraper.git
    cd Cybernaut-Project-Indeed-Web-Scraper
    ```

2.  **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Configure Environment Variables**

      - Sign up or log in to your [Apify account](https://apify.com/).
      - Go to the [Apify Indeed Scraper](https://apify.com/apify/indeed-scraper) actor page.
      - Navigate to the **API** tab to find your **Personal API Token** and the **Actor ID**.
      - Create a file named `.env` in the root of the project and add your credentials:

    <!-- end list -->

    ```ini
    # .env
    APIFY_TOKEN="your_personal_api_token"
    ACTOR_ID="your_actor_id_for_indeed_scraper"
    ```

### 💻 How to Run

1.  Execute the script from your terminal:
    ```bash
    python job_scraper.py
    ```
2.  When prompted, enter the job title you want to search for (e.g., `Python Developer`).
3.  The script will run the Apify actor and save the results in a file named `output.csv`.

-----

## 📊 Sample Output (`output.csv`)

| Job Title | Company | Location | Salary | Job Type | Rating | Reviews | Posted | Apply Link | Description |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Python Developer | XYZ Pvt Ltd | Chennai | ₹8L-12L | Full-time | 4.2 | 123 | 2 days ago | `apply_link_here` | `Cleaned job text...` |
| Data Scientist | ABC Corp | Bengaluru | ₹10L-15L| Full-time | 4.5 | 450 | 5 days ago | `apply_link_here` | `Cleaned job text...` |

-----

## ⚠️ Important Notes

  - **First Run Delay**: The initial run might take up to a minute as Apify initializes the actor and performs the scrape in the background.
  - **Apify Credits**: Be mindful of your Apify usage, as free accounts have a limited number of credits.
  - **Security**: Never commit your `.env` file or expose your API keys in your version control history.

-----

## 👤 Author

**Karthick S**

  - **GitHub**: [@Karthih2](https://github.com/Karthih2)
