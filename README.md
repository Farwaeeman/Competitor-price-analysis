# Competitor Pricing Analysis: Supabase vs Firebase vs Appwrite

An internship project (internee.pk) that compares the pricing, offerings and user engagement of three backend platforms for app developers. The results are used to support pricing decisions.

## Assumption
The task did not name an industry or competitors, so I chose three backend platforms: Supabase, Firebase and Appwrite.

## Data sources
- **User engagement:** GitHub stars, forks and open issues from the public GitHub API.
- **Pricing and offerings:** each pricing page was checked against robots.txt, downloaded with requests and BeautifulSoup, and searched for prices. Plan names, prices and limits were confirmed by reading the pages and entered into tables.
- Data was collected on 2-3 October 2026.

## Key findings
- Supabase and Appwrite start at $25 per month. Firebase has no fixed fee and charges for usage only.
- The cheapest platform depends on app size: Firebase below about 110 GB stored, Appwrite from about 110 to 2,200 GB, and Supabase above about 2,200 GB (assuming data transfer is 2 x storage).
- Appwrite includes the most storage, data transfer and active users in its Pro plan.
- Supabase has the most developer interest on GitHub.

## Charts
![Cost scenarios](charts/chart_4_cost_scenarios.png)
![Cost curve](charts/chart_6_cost_curve.png)
![Features](charts/chart_7_features.png)

## Files
- `Competitors_Pricing_Analysis.ipynb`: the full analysis (code, outputs and notes)
- `Competitor_Pricing_Analysis_Report_Final.pdf`: the written report
- `data/`: the collected tables and downloaded pricing page text
- `charts/`: all charts

## How to run
1. Install the libraries: `pip install -r requirements.txt`
2. Open the notebook in Jupyter and choose Kernel, then Restart & Run All.

## Limitations
- Only three competitors were compared.
- Costs include storage and data transfer only.
- The app sizes and the data transfer ratio are my own examples.
- Prices change often and may be different after 3 October 2026.

## Author
Farwa Eeman
