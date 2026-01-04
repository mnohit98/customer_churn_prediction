# Dataset Download Instructions

## How to Download the Customer Data

1. **Open the Google Sheets link:**
   https://docs.google.com/spreadsheets/d/1rnBO9F9xdSUY-WpeOJilMxMRZT-hwwWq6O98OHreY0k/edit?gid=1602415961#gid=1602415961

2. **Download as CSV:**
   - Click on **File** → **Download** → **Comma Separated Values (.csv)**

3. **Save the file:**
   - Save the downloaded file as `customer_data.csv`
   - Place it in the `data/` folder of this project
   - Final path should be: `data/customer_data.csv`

4. **Verify the file:**
   - The CSV file should contain columns like:
     - customerID, gender, SeniorCitizen, Partner, Dependents
     - tenure, PhoneService, MultipleLines, InternetService
     - OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport
     - StreamingTV, StreamingMovies, Contract, PaperlessBilling
     - PaymentMethod, MonthlyCharges, TotalCharges, Churn

## Alternative: Manual Data Entry

If you cannot download from Google Sheets, you can manually create the CSV file with the same column structure as shown in the Google Sheets.

## Note

Make sure the file is named exactly `customer_data.csv` and placed in the `data/` directory before running the notebooks.

