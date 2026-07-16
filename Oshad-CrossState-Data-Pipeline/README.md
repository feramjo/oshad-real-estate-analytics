# Multi-Source Cross-State Transactional Data Ingestion Pipeline

## 📊 Business Context & Challenge
As Oshad & Co Real Estate scaled operations from its Ibadan headquarters into high-volume national hubs (Lagos, Abuja FCT, Rivers, Ogun, and Osun), the core transaction database grew to thousands of rows but suffered from extreme data corruption due to manual user entry at satellite branches. 

The raw database registry suffered from overlapping string keys (e.g., `'Agent Alao'`, `'agent alao'`, `'Agent Okon '`), inconsistent property transaction statuses (`'SOLD'`, `' sold'`), and unpopulated null parameters within valuation fields due to logging dropouts. This data fragmentation paralyzed monthly multi-state auditing and corporate financial transparency.

## 🛠️ Advanced Data Mechanics Applied
*   **Power Query Automated ETL Engine:** Programmed a multi-source data ingestion pipeline. Leveraged custom string-cleansing routines—including cell trimming, case-matching logic, and column text-parsing filters—to scrub 3,500 raw records into identical corporate entries.
*   **Dynamic Null-Value Treatment:** Configured advanced validation steps within Power Query to isolate missing variables inside `Market_Value_NGN` data fields, automatically computing and applying conditional baseline metrics to preserve dataset functionality.
*   **Standardized Production Output:** Cleaned and compiled a fractured 3,500-row registry into a clean, unified relational table format, slashing manual cross-state reporting times by 85%.

## 🎯 Production Deliverable
The final product is an Automated Data Cleaning Pipeline Template (`Oshad_Properties_CrossState_Raw_Registry_2025.xlsx`). When a user refreshes the data connection via Power Query, it transforms thousands of broken rows into a perfectly cleaned, standardized master sheet instantly.
