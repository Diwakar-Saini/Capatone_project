# Dynamic Pricing for Urban Parking Lots
**Summer Analytics 2025 Capstone Project**  
[![Open in Colab to see the results for model 1 the file is just demo code here see the corrected version](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1b7z16bDHggoQxfWTA0CZQKBJoIjTwAkQ?usp=sharing)

## 📌 Project Overview
Implements dynamic pricing models for 14 urban parking lots using real-time data streams. This repository contains Model 1 (Baseline Linear Model) as described in the problem statement.

## 🧠 Model 1: Baseline Linear Model
**Pricing Formula**:  
`Price_{t+1} = Price_t + α × (Current Occupancy / Capacity)`  

**Implementation**:
- Starts from **$10 base price**
- Updates price daily
- Scales linearly with occupancy fluctuations

## ⚙️ Technical Stack
- **Stream Processing**: Pathway
- **Visualization**: Bokeh + Panel
- **Core Libraries**: Pandas, NumPy
- **Environment**: Google Colab

## 🚀 Setup & Execution
1. **Open in Colab**:  
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1b7z16bDHggoQxfWTA0CZQKBJoIjTwAkQ?usp=sharing)
2. **Upload dataset.csv** when prompted
3. **Run all cells** sequentially

## 📊 Key Visualizations
![Sample Dashboard](screenshot.png)  
*Real-time price tracking across parking lots*

## 🧩 Model Components
| Component          | Functionality                             |
|--------------------|-------------------------------------------|
| Data Preprocessing | Cleans and structures raw parking data    |
| Streaming Engine   | Simulates real-time data ingestion        |
| Pricing Model      | Computes daily price updates              |
| Visualization      | Interactive dashboard of price evolution |

## 📂 File Structure
 ```
    ├── dataset.csv # Sample parking data
    ├── Dynamic_Pricing_Model1.ipynb # Main Colab notebook
    ├── parking_stream.csv # Processed streaming data
    └── README.md # Project documentation
 ```

## 📝 Report Insights
- **Demand Function**: Linear scaling with occupancy rate
- **Assumptions**: 
  - Daily price updates sufficient for baseline
  - Capacity remains constant
- **Price Sensitivity**: 
  - +0.7% price change per 1% occupancy fluctuation

## 🔜 Next Steps
1. Implement **Model 2** (Demand-based pricing)
2. Add competitor price integration (**Model 3**)
3. Incorporate rerouting suggestions

---
**Capstone Project for Summer Analytics 2025**  
[Consulting & Analytics Club × Pathway](https://www.caciitg.com/sa/course25/)
