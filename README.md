## Car Market Trend Analysis

1. Background and Overview
- Used car prices vary widely based on vehicle age, mileage, fuel type, ownership history and seller type. Without clear data insights, buyers and sellers struggle to price vehicles accurately.

This project analyzes CarDekho used-car listings to identify the primary drivers of resale value, separating high-impact factors from common market misconceptions.

2. Data Structure Overview
- The analysis utilizes a clean dataset containing 299 unique vehicle records with zero missing values:

- Core Metrics: Selling_Price (Target resale value) and Present_Price (Original showroom price).

- Vehicle Usage: Year (Model year to calculate age) and Kms_Driven (Total mileage).

- Vehicle Specifications: Fuel_Type (Petrol, Diesel, CNG) and Transmission (Manual, Automatic).

- Market Characteristics: Seller_Type (Dealer vs. Individual) and Owner (Number of previous owners).

3. Executive Summary
- Resale prices are primarily dictated by a car’s original price tag and its fuel-transmission configuration rather than mileage alone. High-value listings are concentrated in specific categories, while older cars lose value rapidly before stabilizing past the 15-year mark.

4. Insights Deepdive
- Price Distribution: Most vehicles sell in the ₹0–5L range with a median price of ₹3.60L. A few high-value listings skew the average price to ₹4.66L.

- Depreciation & Age: Prices drop steeply between ages 8 and 15 (~₹9.3L down to under ₹3L). Beyond 15 years, prices fluctuate unpredictably due to low listing volumes.

- Fuel & Transmission Premium: Automatic Diesel vehicles command the highest average resale price (~₹20.5L), significantly outperforming Petrol (~₹3–4.5L) and CNG variants.

- Mileage Brackets: Mileage does not cause a continuous linear price drop; major value loss occurs in discrete brackets, particularly after crossing 75,000–100,000 km.

- Seller Dynamics & Ownership: Single-owner cars hold a distinct premium. Dealer listings average ₹4.98L compared to Individual listings at ₹0.51L, reflecting higher-grade inventory rather than markups alone.

- Top Price Predictor: Original showroom price (Present_Price) holds the strongest correlation (0.80) with final resale price.

5. Recommendations
- Target Premium Inventory: Focus sourcing and acquisition efforts on Diesel Automatic cars under 14 years old to maximize profit margins.

- Bracket-Based Valuations: Use fixed mileage brackets (e.g <50k, 50k-100k, >100k) rather than raw odometer counts to estimate depreciation.

- Cautious Aging Cap: Apply strict risk discounts when pricing vehicles older than 15 years due to market volatility.

6. Assumptions and Limitations
- Sample Size: The dataset represents a localized sample of 299 vehicles, which may not capture full national market variations.

- Condition Data: Physical vehicle condition, accident history and service records were not available in the dataset.

- Inflation: Historical prices are not adjusted for annual inflation.

7. Future Enhancements
- Incorporate predictive machine learning models (e.g  Random Forest Regression) to automate price estimation.

- Integrate dynamic real-time market data to account for seasonal price fluctuations.

- Expand the dataset to include region-specific pricing and vehicle condition scoring.

8. Deliverables
- python/: Jupyter notebooks and Python scripts for data cleaning, exploratory analysis, and chart generation.

- docs/: Presentation-ready slide deck summarizing key business findings for non-technical stakeholders.

- data/: CarDekho dataset used for analysis.

9. Output Demo
  Link : https://github.com/yashmonde24/car-market-insights/tree/main/output
