NYC BROOKLYN ROLLING SALES DASHBOARD
Mini-Project 2 — Khushi Agarwal
======================================

LIVE URL
--------
https://mp2-brooklyn-dashboard.onrender.com
(Note: free tier spins down after inactivity — first load may take ~30 seconds)

LOCAL SETUP
-----------
1. Install dependencies:
   pip install -r requirements.txt

2. Make sure rollingsales_brooklyn.xlsx is in the same folder as final_dashboard.py

3. Run the dashboard:
   python final_dashboard.py

4. Open browser to:
   http://localhost:8050

FILES
-----
final_dashboard.py          — Main dashboard application
rollingsales_brooklyn.xlsx  — NYC Rolling Sales dataset (Brooklyn)
requirements.txt            — Python dependencies
Procfile                    — Render.com deployment config
MP2_Final_Submission.ipynb  — Jupyter notebook version of the dashboard

CHANGES FROM WEEK 7 PROTOTYPE
------------------------------
Fix 1: Active neighborhood name now shown in all 3 view titles
Fix 2: View 2 title split to 2 lines (no more overflow)
Fix 3: View 1 now uses single color / highlight scheme
        (removes misleading 10-color overlap)
Fix 4: Property size range slider added; default upper bound
        is 99th percentile so outlier (~1.6M sqft) is excluded
        on load — users can expand range manually if needed
