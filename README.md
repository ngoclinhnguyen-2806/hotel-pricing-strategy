# Airbnb Dynamic Pricing Strategy with Price Elasticity Analysis

## Overview
A data-driven dynamic pricing system for Airbnb properties that leverages price elasticity analysis and early booking signals to optimize revenue. The system predicts occupancy rates and generates pricing recommendations based on market conditions, demand patterns, and customer price sensitivity.

## Key Features

### 🔍 **Price Elasticity Analysis**
- Analyzes historical booking data to determine market price sensitivity
- **Price Elasticity: -0.05** (Low elasticity - customers less price sensitive)
- Enables aggressive pricing strategies with ±30-40% price adjustments
- Model R²: 0.44 across 2,358 observations

### 📊 **Occupancy Prediction Model**
- Predicts occupancy rates using key features:
 - **Early demand signals** (7-day advance bookings) - *strongest predictor*
 - Weekend nights (+7.5% occupancy boost)
 - High season periods (+12.7% occupancy boost)

### 💰 **Revenue Optimization**
- Automatically calculates optimal pricing multipliers
- Balances price increases with demand sensitivity
- **Result**: Up to 40% price premiums during high-demand periods
- Real-time strategy adjustment based on early booking patterns

## Model Performance
- **Dataset**: 2,358 booking records with comprehensive feature engineering
- **Price Elasticity**: -0.05 (1% price increase → 5% occupancy change)
- **Early Demand Coefficient**: 1.26 (strongest predictor of final occupancy)
- **Market Classification**: Low elasticity market suitable for aggressive pricing

## Sample Results
For a 7-day forecast with varying demand patterns:
- **High demand days** (100% early bookings): đ868,000 optimal price (40% premium)
- **Mixed demand periods**: Dynamic adjustment based on early signals

## Technical Implementation
- **Language**: Python with pandas, scikit-learn, numpy
- **Models**: Linear regression for elasticity, Random Forest for occupancy prediction
- **Features**: Holiday detection, seasonality, weekend patterns, early booking signals
- **Interface**: Interactive fraction input support (e.g., 5/8, 3/4)

## Business Impact
- **Strategic Insight**: Market has low price sensitivity - aggressive pricing recommended
- **Revenue Optimization**: Early booking signals provide 7-day advance revenue forecasting
- **Operational Efficiency**: Weekly adjustment on price settings based on predictive analytics

---

*This system transforms raw booking data into actionable pricing strategies, enabling property owners to maximize revenue through data-driven decision making.*
