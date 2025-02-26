# 📡 Open GNSS Dataset  

This repository provides open-source Global Navigation Satellite System (GNSS) data collected from suburban of Hong Kong. The dataset is useful for GNSS research, positioning applications, and navigation studies.

## 📂 Dataset Contents
- `data/gnss_data.rinex` – GNSS raw observations in RINEX format  
- `data/gnss_data.csv` – Processed GNSS data in CSV format  
- `metadata/experiment_settings.json` – Experiment metadata  
- `images/` – Photos of the experimental setup  

## 🏗 Experiment Details
- **Location:** Tsim Sha Tsui, Hong Kong  
- **Date (UTC):** 13/02/2025
- **Antenna Type:** NovAtel (GPS-703-GGG)
- **GNSS Receiver:** LABSAT 3W  
- **Ground truth:** NovAtel SPAN-CPT + IE, 1Hz

## 📑 Data Format  

| DataSets    | Urban_HK.bin       | Ground Truth Data    |
|-------------|--------------------|----------------------|
| Total Size  | 9.96 GB (87s)      |      443 KB (102s)   |
| Equipments  | LABSAT 3W          | NovAtel SPAN-CPT + IE|
| Antenna     | NovAtel (GPS-703-GGG) | NovAtel (GPS-703-GGG) |

## 🏗 Experiment Details
- **Sampling Frequency:** 58 MHz
- **IF Frequency:** 4.58 MHz
- **Data Format：** 8-bit I/Q samples
- **Observation Type:** GPS L1 


## 📥 Download & Usage  
You can download the dataset directly from the [GitHub repository](https://github.com/yourusername/GNSS-OpenData).  

### **Using the Data**
To process RINEX files, use:  
```bash
teqc +qc data/gnss_data.rinex
