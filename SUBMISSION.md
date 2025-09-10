# USDS eCFR Take-Home Assessment — Submission

## Feedback on the Assignment
This assignment was challenging but a valuable learning experience. It required end-to-end work: downloading live eCFR data, storing it, creating APIs, and building a UI to analyze results. I appreciated how it exercised full-stack skills: API integration, database design, metrics computation, and frontend visualization.  

The hardest part for me was configuring the local environment and debugging why the “Latest per-Title Metrics” table didn’t populate. Once corrected, the system demonstrated ingestion, metrics calculation, and visualization as required.  

In addition to word counts and section counts, I added a **custom readability index metric**. This helps assess the complexity of regulatory text and provides additional decision-making value.  

I believe my skills in interoperability, data governance, and building systems that integrate with federal APIs position me well for this type of work. While I am out of practice coding at this level, I was able to learn, adapt, and deliver a working solution.

## Duration
This project took approximately **8 hours** to complete, including environment setup, coding, and debugging.

## Frontend Link
The frontend is served locally via FastAPI + Uvicorn at:  http://127.0.0.1:8000 
*(Runs locally and demonstrates ingestion, metrics, and charting features.)*

## Screenshots
Screenshots of the working UI are included in the repository under the [`screenshots/`](./screenshots) folder.

- **Screenshot 1:** Ingesting Title 21 (date: 2024-07-01)  
- **Screenshot 2:** Top Agencies, Latest per-Title Metrics, and Historical chart populated

---

