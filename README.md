# 📡 Open GNSS Dataset  

This repository provides open-source Global Navigation Satellite System (GNSS) data collected from [location] during an experiment conducted on [date]. The dataset is useful for GNSS research, positioning applications, and navigation studies.

## 📂 Dataset Contents
- `data/gnss_data.rinex` – GNSS raw observations in RINEX format  
- `data/gnss_data.csv` – Processed GNSS data in CSV format  
- `metadata/experiment_settings.json` – Experiment metadata  
- `images/` – Photos of the experimental setup  

## 🏗 Experiment Details
- **Location:** [Experiment location]  
- **Date:** [YYYY-MM-DD]  
- **GNSS Receiver:** [Model Name]  
- **Antenna Type:** [Antenna Model]  
- **Sampling Rate:** [X Hz]  
- **Observation Type:** [L1, L2, etc.]  
- **Data Format:** [RINEX, CSV, etc.]  

## 📑 Data Format  
### **CSV File Structure**
| DataSets       | GPS IF Data                 | Ground truth Data |
|--------------|-----------------------------|
| Total Size   | 9.96 GB (87s)   |                       |
| Equipments      | LABSAT 3W            | SPAN-CPT          |
| Antenna     | Novetel(GPS-703-GGG)          | Novetel(GPS-703-GGG) |


## 📥 Download & Usage  
You can download the dataset directly from the [GitHub repository](https://github.com/yourusername/GNSS-OpenData).  

### **Using the Data**
To process RINEX files, use:  
```bash
teqc +qc data/gnss_data.rinex
