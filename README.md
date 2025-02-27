# 📡 Open GNSS Dataset  

This repository provides open-source Global Navigation Satellite System (GNSS) data collected from suburban Hong Kong. The dataset is useful for GNSS research, positioning and navigation studies.

## 📂 Dataset Contents
- `GT_20250213_10Hz.txt` – Ground truth data in text format  
- `Urban_HK.bin` – GPS intermediate frequency (IF) data in binary format
- `images/` – Photos of the experimental setup  

## 🏗 Experiment Details
- **Location:** Tsim Sha Tsui, Hong Kong  
- **Date (UTC):** 13/02/2025
- **Antenna Type:** [NovAtel (GPS-703-GGG)](https://novatel.com/support/previous-generation-products-drop-down/previous-generation-products/gps-703-ggg-antenna)
- **GNSS Receiver:** [LabSat 3 Wideband](https://www.labsat.co.uk/index.php/en/products/labsat-3-wideband)
- **Ground truth:** [NovAtel SPAN-CPT](https://novatel.com/products/gnss-inertial-navigation-systems), 10 Hz


<figure>
  <img src="Images/Environment.jpg" alt="Environment" width="800" height="330">
  <figcaption>Figure 1: (a) Equipment setup and (b) test environment in suburban Hong Kong, showing the test trajectory (red arrow) and sky plot. Satellites in
green indicate LOS signals, while those in orange represent multipath interference based on ray-tracing analysis.</figcaption>
</figure>

<figure>
  <img src="Images/User trajectory.gif" alt="User trajectory" height="330">
  <figcaption>Figure 2: User trajectory.</figcaption>
</figure>

## 📑 Data Format
- **Sampling Frequency:** 58 MHz
- **IF Frequency:** 4.58 MHz
- **Data Format：** 8-bit I/Q samples
- **Observation Type:** GPS L1

| DataSets    | Urban_HK.bin       | GT_20250213_10Hz.txt |
|-------------|--------------------|----------------------|
| Total Size  | 9.96 GB (87s)      |      443 KB (102s)   |
| Equipments  | LABSAT 3W          | NovAtel SPAN-CPT, 10 Hz|
| Antenna     | NovAtel (GPS-703-GGG) | NovAtel (GPS-703-GGG) |

## 📥 Download & Usage  
The GPS IF data will be made publicly available upon acceptance of the paper.
You can download the dataset directly from the [GitHub repository](https://github.com/yourusername/GNSS-OpenData).  

### **Citation**
If you use this work for your research, you may want to cite:  
```bash
TBC
