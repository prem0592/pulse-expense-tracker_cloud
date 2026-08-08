# pulse-expense-tracker_cloud
Daily Expense Tracker with Cloud Storage
[README.md](https://github.com/user-attachments/files/30855743/README.md)
# Pulse Cloud Sync

This version synchronizes the same Pulse account between iPhone and laptop.

## 1. Create a Supabase project
Create a free Supabase project and copy:
- Project URL
- anon/publishable key

Do NOT use a `service_role` key in the app.

## 2. Create the database
Open Supabase → SQL Editor and run `supabase_schema.sql`.

The schema enables Row Level Security so each account can access only its own expenses/templates.

## 3. Run the app
Open `index.html` from an HTTPS host (GitHub Pages is suitable), click **Cloud Setup**, enter the Project URL and anon/publishable key, then create/sign in to your Pulse account.

Use the same account on the phone and laptop.

## 4. Import existing data
Your historical data is intentionally NOT included in the public app.
Use the separate private CSV backup:
`Pulse_PRIVATE_expenses_backup.csv`
Import it after signing in. The rows will be uploaded to your cloud account.

## 5. GitHub
Upload only:
- index.html
- supabase_schema.sql (optional; not needed by the browser)
- no private CSV

The app uses the Supabase anon key in the browser. Security comes from Supabase Auth + RLS, not from hiding the anon key.
