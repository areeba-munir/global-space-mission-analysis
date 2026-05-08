#  Global Space Mission Analysis (1957 – 2020)

###  Project Motivation: Why do this?
Space exploration has transitioned from a government-led "prestige" race into a multi-billion dollar commercial industry. This project explores 60+ years of mission data to understand the **geopolitical shifts** in space dominance, the **economic evolution** of launch costs, and the **engineering progress** of mission reliability. By visualizing these trends, we can see how humanity's access to the stars has fundamentally changed.

---

###  Technical Implementation (The Workflow)
I built a comprehensive data pipeline using **Python** to transform raw, semi-structured mission records into actionable insights.

1.  **Data Wrangling & Standardization:**
    * **Geographic Mapping:** Extracted country names from messy location strings and implemented **ISO-3166 alpha-3** codes for accurate global mapping.
    * **Financial Cleaning:** Standardized mission costs into numeric formats, accounting for currency variations and missing values.
    * **Temporal Formatting:** Parsed inconsistent datetime strings into a uniform format to enable longitudinal time-series analysis.
2.  **Advanced Visualizations (Plotly):**
    * **Choropleth Maps:** Visualizing global launch density and failure hotspots.
    * **Sunburst Charts:** Representing the hierarchical relationships between Country → Organisation → Mission Status.
    * **Rolling Averages:** Applied 5-year and 12-month smoothing to identify long-term trends amid "clumpy" launch data.

---

###  Key Insights & Patterns

#### 1. The Geopolitical "Passing of the Torch"
* **Insight:** The data captures the sharp decline of the Soviet Union’s dominance in 1991. 
* **Trend:** From 2015 onwards, a "New Space Race" emerges. While the 20th century was a bipolar monopoly (USA/USSR), the 21st century is defined by the rise of **China (CASC)** and **Private Enterprise (SpaceX)**.

#### 2. The "SpaceX Effect" on Economics
* **Insight:** Average launch prices reached their historical peak in the 1980s and 90s, driven by complex, non-reusable heavy-lift vehicles like the Space Shuttle.
* **Pattern:** Since 2010, the "Average Price" has crashed by nearly **8x**. This marks the first period in history where space access became cheaper while technological capability increased.

#### 3. The Engineering Learning Curve
* **Insight:** In the late 1950s, the failure rate was as high as **40%**. 
* **Pattern:** Reliability reached a "maturity plateau" in the 1990s. Today, the failure rate hovers around **5%**. This represents the "physical floor" of reliability for modern chemical rocketry.

#### 4. Seasonal & Political Launch Windows
* **Insight:** Launch frequency is not uniform; it follows both climate and fiscal patterns.
* **Pattern:** **December** and **June** show consistent spikes. This highlights the influence of Northern Hemisphere summer weather and political "budget-burn" cycles where agencies rush to complete missions before the end of the fiscal year.

---

###  Repository Structure
* 📁 **`data/`**: Contains the raw and processed CSV datasets.
* 📁 **`notebooks/`**: The Google Colab/Jupyter notebook containing all Python logic and interactive Plotly code.
* 📁 **`images/`**: Static exports of key interactive visualizations for quick viewing.
* 📄 **`requirements.txt`**: List of dependencies (Pandas, Plotly, NumPy) to ensure reproducibility.

---

### 🏁 Conclusion
The transition from an **era of exploration** (1960-1990) to an **era of infrastructure** (2000-Present) is now mathematically evident. The data proves that reusability and commercialization are successfully lowering the barrier to entry, paving the way for the next generation of deep-space exploration.
