# **Analyzing Post-Pandemic Music Trends Using Audio Features** 🎵  

## **Project Overview**  
The COVID-19 pandemic profoundly impacted people's emotions, behaviors, and entertainment preferences. This project aims to **analyze whether U.S. listeners shifted from upbeat, high-energy music to more mellow genres after the pandemic**.  

By leveraging **Spotify and Apple Music APIs**, we extracted key **audio features** from the **top-streamed songs of 2019 (pre-pandemic), 2022, and 2023 (post-pandemic)** to assess changes in musical preferences. Using **statistical analysis and classification models**, we evaluated shifts in:  
- **Energy** ⚡  
- **Valence (positivity of music)** 😊  
- **Acousticness** 🎸  
- **Loudness** 🔊  
- **Mode (major/minor key)** 🎼  

Our findings challenge the assumption that listeners gravitated toward sadder music post-pandemic, revealing **no statistically significant changes in audio features** over time.  

## **Table of Contents**  
- [Project Overview](#project-overview)  
- [Dataset](#dataset)  
- [Methodology](#methodology)  
- [Key Findings](#key-findings)  
- [Technical Implementation](#technical-implementation)  
- [Results & Performance](#results--performance)  
- [Installation & Usage](#installation--usage)  
- [Technologies Used](#technologies-used)  
- [Contributors](#contributors)  
- [Future Work](#future-work)  
- [License](#license)  

---

## **Dataset** 📊  
- **Source:** Spotify & Apple Music APIs  
- **3 datasets (CSV files)** containing the **top 100 streamed songs** for 2019, 2022, and 2023  
- **11 key audio features** per song (energy, valence, acousticness, loudness, tempo, etc.)  
- **Target variable:** Classification of songs as **"upbeat" or "sad"** based on predefined metrics  

---

## **Methodology** 🔍  
1. **Data Collection & Cleaning**  
   - Extracted top 100 streamed songs per year using **Spotify & Apple Music APIs**  
   - Processed data using Python (Pandas, NumPy)  
   - Standardized features and removed anomalies  

2. **Exploratory Data Analysis (EDA)**  
   - Visualized distributions of key audio features across years  
   - Identified trends in **musical characteristics before and after the pandemic**  

3. **Hypothesis Testing (Statistical Analysis)**  
   - **Null Hypothesis:** No significant difference in audio features between years  
   - **Alternative Hypothesis:** Music trends changed significantly post-pandemic  
   - Conducted **t-tests (for continuous variables)** and **z-tests (for binary variables like Mode)**  

4. **Classification Modeling**  
   - Defined an **upbeat vs. sad classification system** using 11 key audio metrics  
   - Applied a **+1, 0, -1 scoring system** to classify songs  
   - Used proportion z-tests to determine if **the percentage of upbeat songs changed significantly**  

---

## **Key Findings** 📌  
- **Listeners did not shift towards sadder music after the pandemic**  
- **2022 saw a temporary increase in high-energy music**, with **higher Energy, Loudness, and Mode scores**  
- **In 2023, music trends reversed**, favoring **more acoustic, lower-energy songs**  
- **Hypothesis tests failed to reject the null hypothesis**, meaning **no statistically significant change** in music preferences  
- **Classification models confirmed that the percentage of upbeat vs. sad songs remained stable**  

---

## **Technical Implementation** ⚙️  
- **Data Extraction & Cleaning:**  
  - Used **Spotify & Apple Music APIs** to gather music data  
  - Processed CSV datasets with **Pandas & NumPy**  
- **Statistical Analysis:**  
  - Performed **t-tests & z-tests** to evaluate significant changes  
- **Classification Modeling:**  
  - Developed **an 11-feature classification system** to label songs as **upbeat or sad**  
  - Evaluated proportions of upbeat music across years  
- **Data Visualization:**  
  - Used **Matplotlib & Seaborn** to generate trend graphs  

---

## **Results & Performance** 📈  
| Feature   | 2019 Mean | 2022 Mean | 2023 Mean | Statistical Significance (p-value) |  
|----------|----------|----------|----------|---------------------------------|  
| **Energy** | 0.74  | 0.76  | 0.73  | 0.21 (Not Significant) |  
| **Valence** | 0.57  | 0.59  | 0.55  | 0.18 (Not Significant) |  
| **Acousticness** | 0.22  | 0.19  | 0.26  | 0.12 (Not Significant) |  
| **Loudness

---

## **Contributors** 👨‍💻👩‍💻 
- Christiaan Kenjee Koh (Project Manager, Data Analyst)
- Dennis Wu (Data Analyst)
- Vy Nguyen (Data Analyst)
- Cyan Huang (Data Analyst)
- Becky Wang (Data Analyst)
