```markdown
# Indeed Scraper using Apify

This project scrapes job postings from **Indeed** using the **Apify Indeed Scraper**.  
It fetches job details (title, company, location, salary, job type, rating, reviews, posted date, apply link, and description) and saves the results into a clean **CSV file** for analysis.

---

## 🚀 Features
- Fetch job postings from Indeed automatically  
- Extracts and cleans job descriptions (removes HTML tags)  
- Saves results in a structured **CSV file**  
- Keeps API keys secure with **.env**  

---

## 📂 Project Structure
```

├── job\_scraper.py         # Main Python script for the scraper
├── .env                   # Stores APIFY\_TOKEN and ACTOR\_ID (not committed to GitHub)
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation

````

---

## 🛠️ Setup & Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/Karthih2/Cybernaut-Project-Indeed-Web-Scraper.git
   cd Cybernaut-Project-Indeed-Web-Scraper
````

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Get your Apify API Token & Actor ID**

   * Go to [Apify Indeed Scraper](https://apify.com/apify/indeed-scraper)
   * Click **Try for free** and sign in (new accounts get free credits)
   * Copy your **API Token** and **Actor ID** from the Apify dashboard

4. **Update your `.env` file**
   Create a `.env` file in the project root (template included):

   ```ini
   APIFY_TOKEN=your_apify_token_here
   ACTOR_ID=your_actor_id_here
   ```

5. **Run the scraper**

   ```bash
   python job_scraper.py
   ```

   Enter the job title you want (e.g., *Python Developer*).
   Results will be saved as:

   ```
   output.csv
   ```

---

## 📊 Example Output

| Job Title        | Company     | Location | Salary  | Job Type  | Rating | Reviews | Posted     | Apply Link        | Description           |
| ---------------- | ----------- | -------- | ------- | --------- | ------ | ------- | ---------- | ----------------- | --------------------- |
| Python Developer | XYZ Pvt Ltd | Chennai  | ₹8L-12L | Full-time | 4.2    | 123     | 2 days ago | apply\_link\_here | Cleaned job text here |

---

## ⚠️ Notes

* The first run may take up to **1 minute** (Apify fetches data in the background)
* Free accounts have limited **credits** on Apify
* Always keep `.env` private and never push API tokens to GitHub

---

## 📧 Author

👤 **Karthick S**
GitHub: [Karthih2](https://github.com/Karthih2)

---
