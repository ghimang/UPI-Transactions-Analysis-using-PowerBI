[⚠️ Suspicious Content] 

💸 UPI Transactions Analysis Dashboard (2024) – Power BI Project.

This Power BI project presents a detailed and interactive analysis of Unified Payments Interface (UPI) transactions for the year 2024, using structured and categorized transaction data to uncover insights and patterns in digital payments across various user demographics, cities, banks, and payment methods.

📂 Dataset Overview
The data used in this report is stored in a single table: UPI Transactions.
It includes the following key fields:

Category	Fields
📊 Transaction Metrics	Amount, RemainingBalance
🏦 Bank Info	BankNameSent, BankNameReceived
🌍 Location	City, Currency
👤 Customer Info	CustomerAccountNumber, CustomerAge, Gender, Age Groups
📱 Device Details	DeviceType
🧾 Merchant Details	MerchantName, MerchantAccountNumber
💳 Payment Info	PaymentMethod, PaymentMode, Purpose, TransactionType
🕒 Transaction Time	TransactionDate, TransactionTime, TransactionID, Status

📊 Dashboard Features
1. Balance by Month (2024)
A column chart visualizing monthly remaining balances.

Shows stable balances between 8.2M and 8.5M across all months.

Toggle buttons to switch between:

Line Chart Amount

Column Chart Amount

Line Chart Balance

Column Chart Balance (Active)

2. City-wise Transaction Summary
Matrix visualization grouped by:

City: Bangalore, Delhi, Hyderabad, Mumbai

Currency: EUR, USD, GBP, INR

Month

Displays Amount and Remaining Balance side-by-side.

3. Dynamic Filtering
Users can explore the data using slicers for:

Bank Names (Sent & Received)

City

Device Type

Gender

Age Groups

Merchant Name

Payment Method

Purpose

Transaction Type

🧠 Insights Uncovered
Transaction stability across months suggests consistent UPI usage.

City-currency trends show varying volumes and balances by region (e.g. high balances retained in Mumbai vs high usage in Delhi).

Analysis can be filtered by:

Customer demographics

Purpose of transaction

Device and payment method types

🛠️ Tools & Tech Used
Power BI Desktop

DAX (Data Analysis Expressions)

Slicer & toggle interactivity

Date hierarchy for monthly analysis

Conditional formatting in matrices

🧪 Sample DAX Measures (if applicable)
dax
Copy
Edit
Total Balance = SUM('UPI Transactions'[RemainingBalance])

Monthly Avg Amount = AVERAGEX(
    VALUES('UPI Transactions'[TransactionDate].[Month]),
    CALCULATE(SUM('UPI Transactions'[Amount]))
)
🚀 How to Use
Download and open the UPI_Transactions.pbix file in Power BI Desktop.

Ensure all slicers and visuals load correctly.

Use the filters to deep dive into specific transactions, user behaviors, and trends.

Explore different visual formats using the chart toggle buttons.

🔮 Future Improvements
Integration of real-time API (NPCI/RBI dashboards).

Add a forecasting trend line using Analytics pane.

Use bookmarks for storytelling dashboards.

Add anomaly detection and outlier alerts for transaction fraud monitoring.

📌 Use Cases
Bank transaction trend analysis

Fintech dashboard for internal analytics

Regional/demographic UPI adoption studies

Merchant performance insights

👨‍💻 Author
Himangsha Goyari
Data Analytics Enthusiast | Special interest in FinTech and BI Tools

