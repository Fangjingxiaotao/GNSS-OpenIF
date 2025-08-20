# 📡 Open GNSS Dataset  

This repository provides open-source Global Navigation Satellite System (GNSS) data collected from urban areas in Hong Kong. The dataset captures the scenario 1 (S1) where a dynamic pedestrian user is moving near a building and the scenario 2 (S2), where a vechile is navigating in a dense urban area. It is valuable for GNSS multipath detection/mitigation research.


## 🏗 Experiment Details
**Scenario 1:**
- **Location:** Tsim Sha Tsui, Hong Kong  
- **Date (UTC):** 13/02/2025

Figure 1 illustrates the experiment setup and test environment of **scenario 1**. It is likely that signals originating from the south are reflected off the building surface, resulting in the reception of both direct and reflected signals. The sky plot in Figure 1(b) presents satellite visibility and signal classification results obtained from ray-tracing techniques. By incorporating user ground truth information, satellite ephemeris, and 3D building models, the ray-tracing algorithm simulates the most probable signal propagation paths. As a result, the analysis indicates that PRN 22 is geometrically susceptible to multipath interference throughout the entire test, while PRN 5 is likely to experience multipath interference during specific epochs of the experiment.
<figure>
  <img src="Images/Environment_S1.jpg" alt="Environment_S1" width="800" height="330">
  <figcaption>Figure 1: (a) Test environment in suburban Hong Kong, showing the test trajectory (red arrow) and sky plot. Satellites in
green indicate LOS signals, while those in orange represent multipath interference based on ray-tracing analysis (b) Equipment setup.</figcaption>
</figure>

Figure 2 illustrates the pedestrian's motion pattern. The pedestrian moves back and forth perpendicular to the building surface for several reasons. First, this motion increases the velocity projection onto the signal path, thereby amplifying the Doppler shift of the reflected signal. Second, the time-varying nature of the reflected signal’s Doppler shift helps characterize its impact on receiver measurements, providing valuable insights into multipath interference effects.
<figure>
  <img src="Images/User trajectory_S1.gif" alt="User trajectory" height="300">
  <figcaption>Figure 2: User trajectory.</figcaption>
</figure>

-----------------------------------------------------------------------------------------------------

**Scenario 2:**
- **Location:** Mong KoK, Hong Kong  
- **Date (UTC):** 06/03/2025

Figure 3 illustrates the experiment setup and test environment of **scenario 2**. This scenario introduces rapid satellite–receiver geometry changes, frequent signal blockages, and high noise levels caused by user dynamics. In our results, several epochs of multipath interference are detected by the ray-tracing with supporting evidence from identifiable reflection geometry. While such intervals are brief, they are sufficient to demonstrate that the proposed estimator converges reliably and is capable of fitting the observed Doppler oscillation behavior.
<figure>
  <img src="Images/Environment_S2.jpg" alt="Environment_S2" width="800" height="330">
  <figcaption>Figure 3: (a) test environment in urban Hong Kong, showing the test trajectory (pink icons) and sky plot. (b) Equipment setup.</figcaption>
</figure>


## 📂 Dataset Contents
- `S1_GT_20250213_1Hz.txt` – Ground truth data of scenario 1 in text format (not yet available)
- `S2_GT_20250603_1Hz.txt` – Ground truth data of scenario 2 in text format (not yet available)
- `S1_suburban_HK.md` – Link to download the GPS intermediate frequency (IF) data of scenario 1
- `S2_urban_HK.md` – Link to download the GPS IF data of scenario 2
- `images/` – Photos of the experimental setup

## 📑 Data Format
For IF data:
- **Sampling Frequency:** 58 MHz
- **IF Frequency:** 4.58 MHz
- **Data Format：** 8-bit I/Q samples
- **Observation Type:** GPS L1

| DataSets    | S1_GT_20250213_1Hz.txt       | S2_GT_20250603_1Hz.txt | S1_suburban_HK.bin | S2_urban_HK.bin|
|-------------|------------------------------|------------------------|--------------------|----------------|
| Total Size  | 40 KB                        |      49 KB             |        9.9GB       |       11 G     |
| Equipments  | NovAtel SPAN-CPT             | NovAtel SPAN-CPT       |   LABSAT 3W        | LABSAT 3W      |
| Antenna     | NovAtel (GPS-703-GGG)                                                                       | 

- **Antenna Type:** [NovAtel (GPS-703-GGG)](https://novatel.com/support/previous-generation-products-drop-down/previous-generation-products/gps-703-ggg-antenna)
- **GNSS Receiver:** [LabSat 3 Wideband](https://www.labsat.co.uk/index.php/en/products/labsat-3-wideband)
- **Ground truth:** [NovAtel SPAN-CPT](https://novatel.com/products/gnss-inertial-navigation-systems), 1 Hz


## 📥 Download & Usage  
The Ground truth data will be made publicly available upon publication of the paper.
You can download the GPS IF data of scenario 1 directly from the [S1_suburban_HK.bin](https://www.dropbox.com/scl/fi/o18ejryo123upfvks5s7w/Urban_HK.bin?rlkey=kxjpoz51fv3lzg8lnnrkk2sqe&st=4u7w5bqw&dl=0).
For questions or further details, please contact: [jingxiaotao2.fang@connect.polyu.hk](mailto:jingxiaotao2.fang@connect.polyu.hk)

### **Citation**

If you use this work for your research, you may want to cite:  
```bash
TBC

