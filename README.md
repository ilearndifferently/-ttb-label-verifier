Installation & Execution:
 1. Ensure Python 3.9+ is installed.
 2. Install dependencies: pip install streamlit rapidfuzz
 3. Run the application: streamlit run app.py

Design Decisions & Assumptions:
UI/UX: Built with Streamlit to ensure a clean, zero-learning-curve interface suitable for all technical comfort levels.

Batch Processing: 
Utilized Streamlit's accept_multiple_files parameter to allow drag-and-drop processing of hundreds of files at once.

Matching Algorithms: 
Split the matching logic into two streams: 
RapidFuzz handles harmless capitalization and punctuation differences for brand names, 
while exact RegEx ensures the Government Warning strictly adheres to federal formatting requirements.