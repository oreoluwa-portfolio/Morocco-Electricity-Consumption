# Morocco-Electricity-Consumption
## Project Overview
* This project focuses on analyzing electricity consumption pattern across three geographical zones in Morocco using python. It explores how electricity consumption changes over time and investigates possible relationships between electricity consumption and environmental factors such as Temperature,Humidity,Windspeed.
 ## Dataset Description
  * This dataset contains approximately 52,416 records  covering January to December 2017, with electricity reading recorded at 10 minutes interval.
    ## Tools
    * Python
    * Google Colab/Jupyter Notebook
    * Pandas
    * Numpy
    * Seaborn
    * Plotly
## Project Workflow
* Task 1: Data Importation and Exploration
* Task 2: Data Cleaning and Preparation
* Task 3:Electricity Consumption Analysis
* TASK 4: Environmental Consumption Analysis
* Task 5: Data Visualisation
* Task 6: Business Insight and Recommendation.
  ## Deliverables
 * Task 1 - 4: https://colab.research.google.com/drive/1bX2-ZJlDdAy0vgYPDOgz3OthdeHrotvr?usp=sharing
 * Task 5: https://docs.google.com/document/d/16OoqKSSFGtSRyDXzZ5ro82nq4QDpmAQ9/edit?usp=drive_link&ouid=101025959233680424055&rtpof=true&sd=true
---

### 1. Key Findings
* **Zone-Based Consumption Profiles:**
  * **Zone 1** is the dominant consumer of electricity, with a high average consumption (~32,345 kW).
  * **Zone 2** exhibits intermediate consumption (~21,043 kW).
  * **Zone 3** maintains the lowest overall footprint (~17,835 kW).
* **Hourly Patterns:**
  * Daily electricity demands demonstrate a distinct U-shaped curve. Peak consumption across all zones begins climbing around late afternoon (17:00) and hits its highest peak in the evening between **19:00 and 21:00**.
  * Off-peak hours occur late at night and early in the morning, hitting a baseline minimum around **04:00 to 06:00**.
* **Weekly Patterns:**
  * Electricity consumption remains consistently high during the weekdays (Monday through Friday) and drops to its weekly minimum on **Sunday**, driven by reduced commercial and industrial activity.
* **Monthly Trends:**
  * Consumption spikes drastically during the summer season, peaking in **July and August** (coinciding with extreme heatwaves and increased cooling demand).
  * Interestingly, Zone 3 shows a massive surge in July, outperforming Zone 2, which suggests a high concentration of tourist activity, seasonal population growth, or temperature-sensitive infrastructure in that specific zone.
* **Environmental Influences:**
  * **Temperature** has a moderate to strong positive correlation with electricity demand ($r \approx 0.38$ to $0.49$). This confirms that cooling loads (air conditioning) significantly drive the grids.
  * **Humidity** is negatively correlated with consumption ($r \approx -0.23$ to -0.29), while **Wind Speed** has a weak positive correlation ($r \approx 0.15$ to $0.28$).

---

### 2. Deep Insights
* **The Cooling Load Dilemma:** The moderate-to-strong positive correlation between Temperature and electricity consumption (especially the massive summer peaks) indicates that cooling/air-conditioning is the single largest weather-related pressure point for the grid.
* **Infrastructure and Demographics:** The dramatic difference in consumption ranges between Zone 1 and the other zones suggests structural variations (e.g., Zone 1 is likely a highly industrialized or dense urban metro center, whereas Zone 3 might be more residential, rural, or highly seasonal/coastal).
* **The Evening Peak Challenge:** Regardless of the zone or the season, there is a recurring daily peak between 19:00 and 21:00. This is likely driven by residential transition (people returning home, turning on appliances, lighting, and cooling simultaneously), putting severe strain on the power grid during these specific hours.

---

### 3. Recommendations
* **Implementation of Demand-Side Management (DSM):** 
  * Introduce **Time-of-Use (ToU) pricing models** to incentivize commercial and residential consumers to shift non-essential operations away from the evening peak hours (19:00–21:00) to off-peak slots (00:00–06:00).
* **Targeted Regional Grid Upgrades:**
  * Priority grid maintenance and expansion should target **Zone 1** to prevent overloading, given its consistently high baseline. 
  * For **Zone 3**, infrastructure must be optimized to handle severe seasonal surges during mid-summer months without sustaining voltage drops.
* **Renewable Energy Integration (Solar and Wind):**
  * Because the highest demand spikes correlate directly with peak daytime temperatures and sunlight hours during summer, **Solar PV generation** is highly suited to offset these cooling peaks.
  * Since wind speed has a positive correlation with consumption, utilizing complementary wind farms can assist during evening peaks when solar generation drops off.
* **Energy Efficiency Programs:**
  * Launch targeted public campaigns and subsidies for high-efficiency HVAC (cooling) systems, particularly in Zone 1 and Zone 2, to flatten the temperature-driven consumption spikes.
