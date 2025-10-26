#  Simple Finance Dashboard

A lightweight Streamlit-based Finance Tracker App that helps you analyze your personal bank transactions, categorize expenses, and visualize spending patterns using interactive charts.

This project automatically categorizes transactions (like Shopping, Travel, etc.) using keywords and lets you manually edit or add categories dynamically — all changes are saved for future uploads.

---------------------------------------------------------------------------------------------------------

##  Features :

✅ Upload CSV Bank Statements
Upload your transaction file (e.g., from your bank portal).

✅ Automatic Categorization
Transactions are automatically categorized based on keywords stored in `categories.json`.

✅ Editable Dashboard
Manually adjust categories directly in the app and have them saved automatically for future sessions.

✅ Dynamic Category Management
Add new categories or keywords within the app itself — no code changes needed.

✅ Interactive Visuals with Plotly
See expense distribution with interactive pie charts.

✅ Real-Time Metrics
Instant summary of total payments and categorized spending.

---------------------------------------------------------------------------------------------------------

##  Technologies Used :

* Python 3.10+
* Streamlit – UI and app interactivity
* Pandas – Data manipulation
* Plotly Express – Data visualization
* JSON – Category data persistence
* OS – File handling

---------------------------------------------------------------------------------------------------------

##  Project Structure :

```
 simple-finance-dashboard
│
├── app.py                    
├── categories.json             
├── sample_bank_statement.csv   
└── README.md                   
```

---------------------------------------------------------------------------------------------------------

##  How It Works :

1. Upload your **bank transaction CSV.
2. The app reads and cleans your data (`Date`, `Amount`, `Details`, `Debit/Credit`).
3. Transactions are categorized automatically using keywords from `categories.json`.
4. You can:

   * Add new categories
   * Edit or reassign categories
   * Save changes (updates `categories.json`)
5. View:

   * Expense summary table
   * Pie chart of category distribution
   * Payment (Credit) summary

---------------------------------------------------------------------------------------------------------

##  Installation & Setup :

### 1️⃣ Clone this repository

```bash
git clone https://github.com/yourusername/simple-finance-dashboard.git
cd simple-finance-dashboard
```

### 2️⃣ Create a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows
```

### 3️⃣ Install dependencies

```bash
pip install streamlit pandas plotly
```

### 4️⃣ Run the app

```bash
streamlit run app.py
```

---------------------------------------------------------------------------------------------------------

##  Usage Tips :

* You can **add new categories** directly in the sidebar tab.
* When you change a transaction’s category, its **details keyword** automatically gets saved for future auto-categorization.
* Your custom categories persist in `categories.json`.

---------------------------------------------------------------------------------------------------------

##  Output Example

Expense Summary Table:

| Category  | Amount (AED) |
| --------- | ------------ |
| Shopping  | 110.69       |
| Insurance | 137.95       |

Pie Chart:

* Interactive visualization of spending by category.

Metrics:

* Total Payments: 18,551.62 AED

---------------------------------------------------------------------------------------------------------

## Future Enhancements :

* Export categorized transactions to Excel
* Multi-file upload support
* Monthly spending trend visualization
* Budget goal tracker

---------------------------------------------------------------------------------------------------------

##  Author :

Rahul Varun
📍 Vizag, India
💼 Passionate about Data Analytics, Automation, and Software Development

---------------------------------------------------------------------------------------------------------

##  License :

This project is open-source under the **MIT License** — feel free to use and modify it.
