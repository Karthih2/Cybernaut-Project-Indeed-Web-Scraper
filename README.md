```markdown
# Job Scraper – Indeed & Apify Integration

A Python-based web scraping tool that collects job postings from Indeed using **Apify Actors**, processes the results, and saves them in structured formats (CSV/Excel).

---

## 📌 Features
- 🔎 Search jobs by **title** and **location**
- ⏳ Limit the number of job postings (e.g., 50 jobs)
- 📊 Saves data into **CSV** for further analysis
- ⚡ Automates data collection with **Apify API**
- 🛡️ Uses `.env` file to keep API keys safe

---

## 🛠️ Tech Stack
- Python 3.9+
- Apify API
- `requests`, `pandas`, `dotenv`

---

## 📂 Project Structure
```

📦 Project Web Scraper
┣ 📜 job\_scraper.py        # Main script
┣ 📜 requirements.txt      # Python dependencies
┣ 📜 .gitignore            # Ignores .env & other unnecessary files
┣ 📜 README.md             # Project documentation
┗ 📜 output.csv            # Sample scraped job postings

````

---

## ⚙️ Setup & Installation
1. **Clone the repository**
   ```bash
   git clone https://github.com/Karthih2/Cybernaut-Project-Indeed-Web-Scraper.git
   cd Cybernaut-Project-Indeed-Web-Scraper
````

2. **Create and activate virtual environment**

   ```bash
   python -m venv venv
   venv\Scripts\activate   # Windows
   source venv/bin/activate  # Linux/Mac
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   Create a `.env` file in the project root:

   ```ini
   APIFY_TOKEN=your_apify_api_token
   ACTOR_ID=your_actor_id
   ```

---

## ▶️ Usage

Run the script:

```bash
python job_scraper.py
```

You’ll be prompted to enter:

* Job Title (e.g., `Python Developer`)
* Location (e.g., `Chennai`)
* Number of job postings to fetch (e.g., `50`)

The results will be saved in `output.csv`.

---

## 📊 Sample Output

| Job Title        | Company     | Location  | Posted | Link                                       |
| ---------------- | ----------- | --------- | ------ | ------------------------------------------ |
| Python Developer | XYZ Pvt Ltd | Chennai   | 1 day  | [https://indeed.com/](https://indeed.com/) |
| Data Engineer    | ABC Tech    | Bangalore | 3 days | [https://indeed.com/](https://indeed.com/) |

---

## 🚀 Future Enhancements

* Add **GUI** for easy usage
* Store data in **databases** (SQL/NoSQL)
* Integration with **email alerts**
* Support for **multiple job sites**

---

## 🛡️ Security

* `.env` is used to store **API tokens**
* **Never commit `.env`** to GitHub
* If you accidentally leak a key, **revoke it immediately**

---

## 🤝 Contributing

Pull requests are welcome. For major changes, open an issue first to discuss what you’d like to change.

---

## 📄 License

This project is licensed under the **MIT License**.

---

👨‍💻 Developed by **Karthick S** (Cybernaut Internship Project)
```
