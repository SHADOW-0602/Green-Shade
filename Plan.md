# Urban Heat Mitigation and Cooling Strategies Platform (Green-Shade)
## Detailed Implementation Plan for ISRO Bharatiya Antariksh Hackathon 2026

**Team Name:** Realm  
**Team Leader:** Kushagra Singh  
**Problem Statement:** Optimizing Urban Heat Mitigation and Cooling Strategies via Artificial Intelligence and Machine Learning (AI/ML)  
**Project Name:** Green-Shade: AI-Driven Urban Heat Mitigation and Cooling Strategy Platform

---

## 1. Executive Summary

Green-Shade is an AI/ML-powered decision-support platform designed to help city planners, municipal teams, and citizens identify urban heat hotspots and choose the most effective cooling strategies. The system combines satellite imagery, weather data, land-use information, IoT/field observations, and population exposure indicators to generate heat-risk maps, forecast future hotspots, simulate cooling interventions, and recommend ranked mitigation actions.

The platform focuses on solving the Urban Heat Island problem, where dense built-up areas, concrete, asphalt, traffic, and limited vegetation cause cities to become significantly hotter than nearby rural areas. Instead of only showing static heat maps, Green-Shade predicts risk, explains why an area is hot, and recommends practical interventions such as tree cover, cool roofs, shaded corridors, reflective roads, water bodies, and public cooling zones.

---

## 2. Problem Background

Urban areas are becoming hotter due to rapid development, loss of vegetation, high building density, dark road surfaces, waste heat from vehicles and air conditioners, and climate change. This creates the Urban Heat Island effect, where city temperatures remain higher during the day and night compared with surrounding rural regions.

### Key Issues

1. **Existing heat maps are mostly descriptive:** They show where heat was observed in the past but do not strongly predict future local heat risk.
2. **Mitigation planning is slow and manual:** Urban planners often need to manually compare maps, climate data, budgets, and feasibility.
3. **Cooling strategies are not optimized together:** Cost, cooling impact, feasibility, and equity are usually considered separately.
4. **Vulnerable populations are often under-prioritized:** High-risk zones with elderly people, children, outdoor workers, low-income groups, and dense settlements need more attention.
5. **Lack of citizen feedback loop:** Local observations such as shaded areas, water availability, and heat discomfort are rarely used to improve models.

---

## 3. Proposed Solution

Green-Shade provides an integrated AI/ML and geospatial platform that performs the following:

1. Collects satellite, weather, land-use, population, IoT, and field data.
2. Processes geospatial data into ward-level or grid-level heat indicators.
3. Predicts current and future heat-risk zones.
4. Classifies hotspots based on severity.
5. Explains the causes of heat risk using model explainability.
6. Simulates cooling interventions.
7. Ranks mitigation strategies based on expected cooling impact, cost, feasibility, and equity.
8. Displays results through an interactive planner dashboard and citizen alert system.

---

## 4. Unique Selling Proposition

Green-Shade is different from a normal heat map because it moves from **observation** to **prediction and decision-making**.

### Differentiators

| Existing Approach | Green-Shade Approach |
|---|---|
| Static heat maps | Predictive heat-risk maps |
| Manual mitigation planning | AI-ranked cooling strategies |
| Focus only on temperature | Includes land use, vegetation, exposure, cost, equity, and feasibility |
| Limited what-if analysis | Simulation of trees, cool roofs, water bodies, shade, and reflective surfaces |
| Planner-only system | Planner dashboard + citizen alerts + feedback |
| Difficult to explain model output | Explainable AI recommendations |

---

## 5. Target Users

### 5.1 City Planner

City planners can select a ward or locality, view heat-risk scores, compare hotspots, simulate interventions, and approve ranked cooling plans.

### 5.2 Municipal Team

Municipal teams can inspect field feasibility, update implementation status, upload before-after data, and track whether cooling actions are working.

### 5.3 Citizens

Citizens can receive heat-risk alerts, find nearby cooling zones, report local heat conditions, and submit feedback that improves future model accuracy.

### 5.4 Disaster Management and Public Health Teams

They can use the platform to identify vulnerable heat-exposure zones and plan emergency responses during heatwaves.

---

## 6. Core Features

### 6.1 AI Heat-Risk Maps

The platform generates ward/grid-level heat-risk maps using:

- Land Surface Temperature (LST)
- NDVI / vegetation index
- NDBI / built-up index
- Albedo or surface reflectance
- Road density
- Building density
- Population exposure
- Weather conditions
- Historical hotspot patterns

Output:

- Heat-risk score from 0 to 100
- Hotspot category: Low, Moderate, High, Severe
- Layer-wise map visualization
- Downloadable map report

### 6.2 Hotspot Forecasting

The system predicts likely high-risk areas for upcoming days or seasons.

Forecasting horizons:

- Same day risk
- Next 24 hours
- Next 3 days
- Seasonal risk trend

Output:

- Forecast heat-risk map
- Expected hotspot probability
- Confidence score
- Alert priority level

### 6.3 Mitigation Optimizer

The optimizer ranks cooling interventions for each ward/grid based on multiple decision factors.

Supported interventions:

- Tree plantation
- Urban parks and green corridors
- Cool roofs
- Reflective road surfaces
- Shaded pedestrian routes
- Water bodies / water mist zones
- Bus-stop shade structures
- Public cooling shelters

Ranking criteria:

- Expected temperature reduction
- Estimated cost
- Implementation feasibility
- Time required
- Population benefited
- Vulnerable population coverage
- Maintenance effort
- Available land or rooftop suitability

### 6.4 What-if Simulator

The planner can test scenarios before implementation.

Example scenarios:

- What if tree cover increases by 15% in Ward A?
- What if 40% of public rooftops are converted into cool roofs?
- What if shaded corridors are added near schools and markets?
- What if reflective surfaces are applied on major roads?

Output:

- Expected temperature reduction
- Cost estimate
- Population benefited
- Equity improvement score
- Before-after map comparison

### 6.5 Planner Dashboard

Dashboard modules:

- Interactive city map
- Ward heat-risk ranking
- Hotspot forecast panel
- Intervention recommendation cards
- Budget vs cooling impact chart
- Equity score chart
- Before-after simulation view
- Downloadable PDF/CSV reports

### 6.6 Citizen Alerts and Feedback

Citizen-side features:

- Local heat-risk alerts
- Suggested cooling zones
- Heat safety tips
- Citizen-reported heat discomfort
- Shade/water availability feedback
- Local issue reporting, such as no shade, high heat, or lack of drinking water

---

## 7. Data Sources

### 7.1 Satellite and Remote Sensing Data

| Data Type | Possible Source | Use |
|---|---|---|
| Land Surface Temperature | ISRO/Bhuvan, satellite thermal bands | Heat map generation |
| NDVI | Satellite imagery | Vegetation density |
| NDBI | Satellite imagery | Built-up intensity |
| Land use / land cover | ISRO/Bhuvan / public GIS datasets | Urban classification |
| Surface reflectance / albedo | Satellite imagery | Heat absorption estimation |

### 7.2 Weather Data

| Data Type | Possible Source | Use |
|---|---|---|
| Air temperature | IMD / OpenWeather | Model input |
| Humidity | IMD / OpenWeather | Heat stress estimation |
| Wind speed | IMD / OpenWeather | Cooling effect |
| Solar radiation | Weather datasets | Surface heating |
| Rainfall | Weather datasets | Seasonal pattern analysis |

### 7.3 Urban and Socioeconomic Data

| Data Type | Use |
|---|---|
| Ward boundaries | Spatial aggregation |
| Road network | Heat exposure and reflective road planning |
| Building footprints | Built-up density |
| Population density | Exposure score |
| Schools, hospitals, markets | Priority locations |
| Public rooftops | Cool roof suitability |
| Open land | Tree/park feasibility |

### 7.4 IoT and Field Data

| Data Type | Use |
|---|---|
| Temperature sensors | Model validation |
| Humidity sensors | Local heat stress detection |
| Citizen feedback | Ground truth improvement |
| Field inspection data | Feasibility validation |

---

## 8. Data Processing Pipeline

### Step 1: Data Collection

- Collect satellite imagery, weather data, GIS boundaries, road networks, building footprints, and population data.
- Store raw data in the data lake or local data folder.

### Step 2: Raster Cleaning

- Remove cloudy pixels.
- Correct missing values.
- Normalize raster resolution.
- Clip imagery to city boundary.

### Step 3: Spatial Grid Creation

- Divide the city into wards or uniform grids, for example 250m x 250m or 500m x 500m.
- Assign all satellite, weather, and urban features to each grid.

### Step 4: Feature Engineering

Features can include:

- Mean LST
- Maximum LST
- NDVI mean
- NDBI mean
- Vegetation ratio
- Built-up ratio
- Road density
- Distance to water body
- Population density
- Historical heat-risk score
- Weather lag features
- Heatwave indicator

### Step 5: Model Training Dataset

Each row represents one grid/ward for one date.

Example columns:

```text
grid_id, date, latitude, longitude, lst_mean, ndvi, ndbi, albedo,
air_temp, humidity, wind_speed, road_density, building_density,
population_density, vulnerable_population, previous_day_temp,
heat_risk_score, hotspot_label
```

### Step 6: Prediction and Recommendation

- ML model predicts temperature/risk.
- Classification model predicts hotspot category.
- Optimizer recommends cooling actions.
- Results are served through APIs and displayed on the dashboard.

---

## 9. AI/ML Methodology

### 9.1 Baseline Models

Baseline models will be used first because they are easier to explain and debug.

- Linear Regression
- Ridge Regression
- Random Forest Regressor
- XGBoost Regressor
- Logistic Regression for hotspot classification
- Random Forest Classifier

### 9.2 Advanced Models

Advanced models can be added after the MVP.

- LSTM for temporal forecasting
- CNN/U-Net for spatial heat pattern extraction
- Graph Neural Network for road/building network heat propagation
- Spatio-temporal transformer for long-term forecasting

### 9.3 Prediction Tasks

| Task | Model Type | Output |
|---|---|---|
| Temperature prediction | Regression | Predicted LST / air temperature |
| Heat-risk scoring | Regression or weighted scoring | 0-100 risk score |
| Hotspot classification | Classification | Low / Moderate / High / Severe |
| Intervention impact estimation | Regression / rule-based model | Expected cooling benefit |
| Priority ranking | Multi-criteria optimization | Ranked actions |

### 9.4 Heat-Risk Score Formula for MVP

For the first prototype, use a transparent weighted formula before advanced ML.

```text
Heat Risk Score =
0.30 × normalized_LST
+ 0.20 × normalized_air_temperature
+ 0.15 × normalized_NDBI
+ 0.15 × normalized_population_exposure
+ 0.10 × normalized_road_density
- 0.10 × normalized_NDVI
```

The weights can later be learned or adjusted using historical data.

### 9.5 Explainable AI

Use SHAP or feature importance to explain why a location is high risk.

Example explanation:

```text
Ward 12 is high risk because:
- Land Surface Temperature is very high.
- Vegetation cover is low.
- Built-up density is high.
- Population exposure is high.
- Wind speed is low.
```

---

## 10. Mitigation Optimization Engine

The optimizer recommends the best cooling actions for each grid or ward.

### 10.1 Inputs

- Heat-risk score
- Hotspot probability
- Existing vegetation
- Built-up density
- Available rooftops
- Road area
- Open spaces
- Population exposure
- Budget limit
- Intervention cost estimates
- Expected cooling impact

### 10.2 Intervention Impact Table for MVP

| Intervention | Expected Cooling Impact | Cost Level | Feasibility Requirement |
|---|---:|---:|---|
| Tree cover increase | High | Medium | Available roadside/open space |
| Cool roof coating | Medium | Low-Medium | Rooftop availability |
| Reflective roads | Medium | High | Road resurfacing feasibility |
| Shade structures | Medium | Medium | Footpath/public place availability |
| Water body restoration | High | High | Land/water availability |
| Cooling centers | Low-Medium | Medium | Public buildings |

### 10.3 Ranking Formula

```text
Priority Score =
0.35 × cooling_impact
+ 0.25 × population_benefit
+ 0.20 × equity_score
+ 0.10 × feasibility_score
+ 0.10 × speed_of_implementation
- 0.20 × normalized_cost
```

### 10.4 Output

For each ward:

```json
{
  "ward_id": "W-12",
  "heat_risk_score": 87,
  "hotspot_level": "Severe",
  "recommended_actions": [
    {
      "rank": 1,
      "action": "Cool roofs on public buildings",
      "expected_temp_reduction": "1.2°C",
      "estimated_cost": "Medium",
      "population_benefited": 42000,
      "equity_score": 0.82
    },
    {
      "rank": 2,
      "action": "Tree plantation near schools and roads",
      "expected_temp_reduction": "1.8°C",
      "estimated_cost": "Medium",
      "population_benefited": 37000,
      "equity_score": 0.78
    }
  ]
}
```

---

## 11. System Architecture

```text
+------------------------------+
|        Data Sources          |
| Satellite, Weather, GIS, IoT |
+--------------+---------------+
               |
               v
+------------------------------+
|   Geospatial Preprocessing   |
| Raster cleaning, cloud mask, |
| grid creation, aggregation   |
+--------------+---------------+
               |
               v
+------------------------------+
|       Feature Store          |
| LST, NDVI, NDBI, roads,      |
| population, weather features |
+--------------+---------------+
               |
               v
+------------------------------+
|        AI/ML Engine          |
| Prediction, classification,  |
| explainability               |
+--------------+---------------+
               |
               v
+------------------------------+
|     Optimization Engine      |
| Cooling action ranking,      |
| cost-impact-equity scoring   |
+--------------+---------------+
               |
               v
+------------------------------+
|        Backend APIs          |
| FastAPI, REST, Auth, Reports |
+--------------+---------------+
               |
               v
+------------------------------+
|       Frontend Dashboard     |
| React, Leaflet, Chart.js     |
+------------------------------+
```

---

## 12. Technology Stack

### 12.1 Frontend

- React with Vite
- TailwindCSS
- Leaflet or Mapbox for map visualization
- Chart.js for charts
- Axios for API calls

### 12.2 Backend

- FastAPI
- Uvicorn
- Pydantic
- REST APIs
- Python services for ML and geospatial processing

### 12.3 AI/ML

- Python
- Pandas
- NumPy
- scikit-learn
- XGBoost
- SHAP for explainability
- PyTorch or TensorFlow for advanced models later

### 12.4 GIS and Data

- GeoPandas
- Rasterio
- Shapely
- PostGIS
- QGIS for manual inspection
- GeoJSON for frontend map layers

### 12.5 Database

MVP option:

- SQLite or JSON files for quick demo

Production option:

- PostgreSQL + PostGIS
- Object storage for raster files

### 12.6 Deployment

- Docker
- Docker Compose
- Cloud VM
- Optional: Render, Railway, AWS, Azure, or GCP

---

## 13. Project Folder Structure

```text
Green-Shade/
├── README.md
├── docker-compose.yml
├── .env.example
├── data/
│   ├── raw/
│   │   ├── satellite/
│   │   ├── weather/
│   │   ├── gis/
│   │   └── field_feedback/
│   ├── processed/
│   │   ├── grids.geojson
│   │   ├── features.csv
│   │   └── heat_predictions.geojson
│   └── sample/
│       └── demo_city_heat_grid.geojson
├── backend/
│   ├── requirements.txt
│   ├── main.py
│   └── app/
│       ├── api/
│       │   ├── heat_maps.py
│       │   ├── forecast.py
│       │   ├── simulate.py
│       │   ├── recommendations.py
│       │   └── feedback.py
│       ├── core/
│       │   ├── config.py
│       │   └── database.py
│       ├── models/
│       │   ├── schemas.py
│       │   └── ml_models/
│       ├── services/
│       │   ├── data_ingestion.py
│       │   ├── geospatial_processing.py
│       │   ├── heat_prediction.py
│       │   ├── optimization_engine.py
│       │   └── report_generator.py
│       └── tests/
├── frontend/
│   ├── package.json
│   ├── index.html
│   └── src/
│       ├── App.jsx
│       ├── main.jsx
│       ├── api/
│       │   └── client.js
│       ├── components/
│       │   ├── HeatMap.jsx
│       │   ├── RiskCard.jsx
│       │   ├── ForecastPanel.jsx
│       │   ├── SimulatorPanel.jsx
│       │   ├── RecommendationCard.jsx
│       │   └── Charts.jsx
│       ├── pages/
│       │   ├── Dashboard.jsx
│       │   ├── Simulator.jsx
│       │   ├── Alerts.jsx
│       │   └── Reports.jsx
│       └── styles/
│           └── index.css
└── notebooks/
    ├── 01_data_exploration.ipynb
    ├── 02_feature_engineering.ipynb
    ├── 03_model_training.ipynb
    └── 04_model_evaluation.ipynb
```

---

## 14. API Design

### 14.1 Health Check

```http
GET /api/health
```

Response:

```json
{
  "status": "ok",
  "service": "Green-Shade API"
}
```

### 14.2 Heat Map API

```http
GET /api/heat-map?city=noida&date=2026-07-01
```

Returns GeoJSON containing heat-risk scores.

### 14.3 Forecast API

```http
GET /api/forecast?city=noida&days=3
```

Returns future hotspot predictions.

### 14.4 Recommendation API

```http
GET /api/recommendations?ward_id=W-12
```

Returns ranked cooling strategies.

### 14.5 Simulation API

```http
POST /api/simulate
```

Request:

```json
{
  "ward_id": "W-12",
  "tree_cover_increase": 15,
  "cool_roof_area_percent": 30,
  "reflective_road_percent": 10
}
```

Response:

```json
{
  "ward_id": "W-12",
  "baseline_heat_risk": 87,
  "new_heat_risk": 72,
  "estimated_temp_reduction": 1.6,
  "estimated_cost": "Medium",
  "population_benefited": 42000
}
```

### 14.6 Citizen Feedback API

```http
POST /api/feedback
```

Request:

```json
{
  "latitude": 28.5355,
  "longitude": 77.3910,
  "heat_discomfort": "High",
  "shade_available": false,
  "water_available": false,
  "comment": "Very hot near bus stop"
}
```

---

## 15. Database Design

### 15.1 Tables

#### city_grid

| Column | Type | Description |
|---|---|---|
| grid_id | string | Unique grid ID |
| ward_id | string | Ward ID |
| geometry | geometry | Polygon boundary |
| area_sq_km | float | Grid area |

#### heat_features

| Column | Type | Description |
|---|---|---|
| id | integer | Primary key |
| grid_id | string | Grid ID |
| date | date | Observation date |
| lst_mean | float | Land surface temperature |
| ndvi | float | Vegetation index |
| ndbi | float | Built-up index |
| air_temp | float | Weather temperature |
| humidity | float | Humidity |
| road_density | float | Road density |
| population_density | float | Population density |

#### heat_predictions

| Column | Type | Description |
|---|---|---|
| prediction_id | integer | Primary key |
| grid_id | string | Grid ID |
| forecast_date | date | Forecast date |
| predicted_temp | float | Predicted temperature |
| heat_risk_score | float | 0-100 score |
| hotspot_label | string | Low/Moderate/High/Severe |
| confidence | float | Model confidence |

#### interventions

| Column | Type | Description |
|---|---|---|
| intervention_id | integer | Primary key |
| name | string | Intervention name |
| cost_level | string | Low/Medium/High |
| expected_impact | float | Expected cooling impact |
| feasibility_rules | json | Conditions for recommendation |

#### recommendations

| Column | Type | Description |
|---|---|---|
| recommendation_id | integer | Primary key |
| grid_id | string | Grid ID |
| intervention_id | integer | Linked intervention |
| priority_score | float | Ranking score |
| estimated_cost | float | Cost estimate |
| expected_temp_reduction | float | Cooling estimate |

#### citizen_feedback

| Column | Type | Description |
|---|---|---|
| feedback_id | integer | Primary key |
| latitude | float | Location |
| longitude | float | Location |
| heat_discomfort | string | Low/Medium/High |
| shade_available | boolean | Shade availability |
| water_available | boolean | Water availability |
| comment | text | Citizen observation |
| created_at | datetime | Submission time |

---

## 16. Frontend Screen Plan

### 16.1 Dashboard Page

Main elements:

- Header with project name and city selector
- Map layer control
- Heat-risk legend
- Ward ranking sidebar
- Hotspot forecast summary
- Top 5 recommended actions
- Download report button

### 16.2 Map Layers

Available layers:

- Heat-risk score
- Land surface temperature
- Vegetation cover
- Built-up index
- Population exposure
- Recommended intervention zone
- Citizen feedback points

### 16.3 What-if Simulator Page

Controls:

- Select ward/locality
- Tree cover increase slider
- Cool roof percentage slider
- Reflective road percentage slider
- Shade structure count input
- Budget limit input

Output:

- Before-after heat-risk score
- Temperature reduction estimate
- Cost-impact chart
- Equity benefit score
- Recommended implementation plan

### 16.4 Alerts Page

- Current high-risk areas
- Forecast severe hotspots
- Citizen safety tips
- Nearby cooling centers
- Alert priority table

### 16.5 Reports Page

- Ward-wise summary
- Model performance metrics
- Intervention comparison
- Export as PDF/CSV

---

## 17. Development Roadmap

### Phase 1: Project Setup

Duration: 1-2 days

Tasks:

- Create monorepo structure.
- Set up FastAPI backend.
- Set up React + Vite frontend.
- Add TailwindCSS.
- Add Docker Compose.
- Create `/api/health` endpoint.
- Create basic dashboard layout.

Deliverables:

- Running frontend and backend.
- Project opens in VS Code.
- Basic API connection working.

### Phase 2: Mock Data MVP

Duration: 3-5 days

Tasks:

- Create sample city grid GeoJSON.
- Generate mock heat-risk scores.
- Build map visualization.
- Add ward ranking sidebar.
- Add risk cards and legend.
- Create mock recommendations.

Deliverables:

- Working heat-risk map.
- Planner dashboard demo.
- Basic recommendation cards.

### Phase 3: Simulation Engine

Duration: 3-5 days

Tasks:

- Build intervention impact formulas.
- Create `/api/simulate` endpoint.
- Add simulator UI sliders.
- Show before-after results.
- Add cost-impact chart.

Deliverables:

- What-if simulation demo.
- Cooling impact results.
- Simple budget trade-off chart.

### Phase 4: ML Model Integration

Duration: 5-7 days

Tasks:

- Create training dataset from mock or real features.
- Train baseline regression model.
- Train hotspot classification model.
- Save model using joblib.
- Add model inference service.
- Add feature importance explanation.

Deliverables:

- Heat prediction model.
- Hotspot classifier.
- Explainable output.

### Phase 5: Real Geospatial Data Integration

Duration: 7-10 days

Tasks:

- Process satellite raster data.
- Calculate NDVI/NDBI/LST features if data is available.
- Aggregate data to grid/ward level.
- Add PostGIS support.
- Replace mock data gradually.

Deliverables:

- Real or semi-real heat-risk layer.
- GIS processing scripts.
- Improved map accuracy.

### Phase 6: Citizen Alerts and Feedback

Duration: 3-5 days

Tasks:

- Create feedback form.
- Save feedback points.
- Display feedback on map.
- Create heat alert logic.
- Add local safety tips.

Deliverables:

- Citizen feedback loop.
- Alert page.
- Feedback-based model improvement plan.

### Phase 7: Reporting and Final Polish

Duration: 3-5 days

Tasks:

- Add PDF/CSV report generation.
- Improve UI design.
- Add loading states and error handling.
- Add mobile responsiveness.
- Prepare final demo script.

Deliverables:

- Final hackathon-ready prototype.
- Demo report.
- Presentation-ready workflow.

---

## 18. MVP Scope

The first working MVP should focus on demonstrating the core idea without waiting for perfect real-world data.

### MVP Must-Have Features

1. Interactive heat-risk map.
2. Ward/grid heat-risk score.
3. Hotspot forecast using mock or sample data.
4. Mitigation recommendation cards.
5. What-if simulator.
6. Dashboard charts.
7. Citizen feedback form.
8. Downloadable summary report.

### MVP Nice-to-Have Features

1. Real satellite raster processing.
2. PostGIS database.
3. Advanced U-Net or LSTM model.
4. SMS/email alerts.
5. Admin login system.

---

## 19. Evaluation Metrics

### 19.1 Temperature Prediction

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R-squared score

### 19.2 Hotspot Classification

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

### 19.3 Recommendation Quality

- Estimated cooling benefit
- Cost-benefit ratio
- Population benefited
- Vulnerable population coverage
- Implementation feasibility score

### 19.4 System Performance

- API response time
- Map loading time
- Dashboard rendering speed
- Feedback submission success rate

---

## 20. Risk Management

| Risk | Impact | Mitigation |
|---|---|---|
| Real satellite data unavailable during MVP | High | Use mock GeoJSON and sample raster data first |
| Cloud cover affects satellite imagery | Medium | Use cloud masking and multiple dates |
| Model accuracy low due to limited data | High | Start with explainable baseline + improve gradually |
| GIS processing becomes complex | Medium | Use QGIS/GeoPandas first, then automate |
| Frontend map becomes slow | Medium | Use simplified GeoJSON or vector tiles |
| Cost estimates are uncertain | Medium | Use relative cost levels first |
| Citizen feedback can be noisy | Medium | Validate and aggregate feedback before using it |

---

## 21. Demo Story for Hackathon

### Demo Flow

1. Open the Green-Shade dashboard.
2. Select a city, for example Noida.
3. Show the AI heat-risk map.
4. Click on a severe hotspot ward.
5. Show why the ward is high risk using explainability.
6. Open recommended cooling actions.
7. Run what-if simulation: increase tree cover and cool roofs.
8. Show expected temperature reduction and cost-impact trade-off.
9. Submit a citizen feedback point.
10. Generate a planner report.

### Suggested Pitch Line

Green-Shade helps cities move from simply seeing heat to actively reducing it using AI-powered prediction, explainable hotspot analysis, and optimized cooling strategies.

---

## 22. Final Deliverables

1. Working web application.
2. FastAPI backend.
3. React planner dashboard.
4. Interactive heat-risk map.
5. Simulation and recommendation engine.
6. Sample dataset or real processed GIS data.
7. ML model notebook.
8. Project README.
9. Docker setup.
10. Final presentation/demo video.

---

## 23. Immediate Next Steps

### Step 1: Confirm MVP City

Recommended city for MVP: **Noida**, because the team is from Amity University, Noida and local context may be easier to explain.

### Step 2: Start with Mock GeoJSON

Create sample wards/grids with generated values for:

- LST
- NDVI
- NDBI
- population density
- heat-risk score
- recommended action

### Step 3: Build Basic Backend

Create FastAPI endpoints:

- `/api/health`
- `/api/heat-map`
- `/api/forecast`
- `/api/recommendations`
- `/api/simulate`
- `/api/feedback`

### Step 4: Build Basic Frontend

Create React pages:

- Dashboard
- Simulator
- Alerts
- Reports

### Step 5: Add ML Gradually

Start with formula-based heat-risk scoring, then add Random Forest/XGBoost once data is ready.

---

## 24. Recommended First Sprint Checklist

- [ ] Create GitHub repository.
- [ ] Create `frontend` using Vite + React.
- [ ] Create `backend` using FastAPI.
- [ ] Add TailwindCSS.
- [ ] Add Leaflet map.
- [ ] Create mock GeoJSON file.
- [ ] Display heat-risk map.
- [ ] Create heat-risk cards.
- [ ] Create recommendations API.
- [ ] Create simulator API.
- [ ] Connect frontend to backend.
- [ ] Prepare README with setup commands.

---

## 25. Suggested Repository Name

```text
green-shade-ai-urban-heat-mitigation
```

Alternative names:

- HeatShield AI
- UrbanCool AI
- CoolCity AI
- ThermalGuard AI
- GreenShade AI

---

## 26. Conclusion

Green-Shade is a practical and scalable solution for urban heat mitigation. It combines satellite intelligence, weather analysis, geospatial processing, AI/ML prediction, and optimization to help cities choose the right cooling strategies in the right places. The MVP can be built quickly using mock geospatial data and then upgraded with real ISRO/Bhuvan and weather datasets for stronger accuracy and real-world usefulness.
