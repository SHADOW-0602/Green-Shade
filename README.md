# Green-Shade: AI-Driven Urban Heat Mitigation and Cooling Strategy Platform

**Bharatiya Antariksh Hackathon 2026**

**Team Name:** Realm  
**Team Leader:** Kushagra Singh

## 🌍 Executive Summary
Green-Shade is an AI/ML-powered decision-support platform designed to help city planners, municipal teams, and citizens identify urban heat hotspots and choose the most effective cooling strategies. The system combines satellite imagery, weather data, land-use information, IoT/field observations, and population exposure indicators to generate heat-risk maps, forecast future hotspots, simulate cooling interventions, and recommend ranked mitigation actions.

## 🌡️ The Problem
Urban areas are becoming hotter due to rapid development, loss of vegetation, high building density, dark road surfaces, waste heat, and climate change. This creates the **Urban Heat Island (UHI)** effect. 
Existing solutions often only describe past heat, lack optimized mitigation planning, and under-prioritize vulnerable populations. Green-Shade moves from mere observation to **prediction and decision-making**.

## 🎯 Target Users
- **City Planners:** View heat-risk scores, simulate interventions, and approve cooling plans.
- **Municipal Teams:** Inspect field feasibility and track implementation impact.
- **Citizens:** Receive heat-risk alerts, find cooling zones, and submit ground-truth feedback.
- **Disaster Management:** Identify vulnerable zones for emergency response during heatwaves.

## ✨ Core Features
- **AI Heat-Risk Maps:** Generates ward/grid-level heat-risk scores using LST, NDVI, NDBI, and population exposure.
- **Hotspot Forecasting:** Predicts likely high-risk areas for upcoming days or seasons.
- **Mitigation Optimizer:** Ranks cooling interventions (e.g., tree cover, cool roofs, reflective roads) based on impact, cost, and equity.
- **What-if Simulator:** Tests scenarios before implementation (e.g., "What if tree cover increases by 15%?").
- **Planner Dashboard:** Interactive city map, hotspot forecast panel, and budget vs. cooling impact charts.
- **Citizen Alerts & Feedback:** Local heat-risk alerts and mechanisms to report heat discomfort or shade availability.

## 🛠️ Technology Stack
- **Frontend:** React (Vite), TailwindCSS, Leaflet/Mapbox, Chart.js
- **Backend:** FastAPI (Python), REST APIs, Uvicorn
- **AI/ML:** Python, Pandas, NumPy, scikit-learn, XGBoost, SHAP (Explainability)
- **Data & GIS:** GeoPandas, Rasterio, PostGIS, QGIS (Data sources: ISRO Bhuvan, OpenWeather)
- **Deployment:** Docker, Docker Compose, Cloud VM

## 🏗️ Getting Started (Coming Soon)
*Instructions on how to set up, build, and run the Green-Shade platform locally using Docker will be added here once development begins.*

## 🛣️ Development Roadmap
- **Phase 1:** Project Setup (Monorepo, FastAPI, React+Vite, Docker)
- **Phase 2:** Mock Data MVP (Interactive maps and dashboard with sample data)
- **Phase 3:** Simulation Engine (What-if formulas and impact charts)
- **Phase 4:** ML Model Integration (Heat prediction and hotspot classification)
- **Phase 5:** Real Geospatial Data Integration (Satellite raster processing)
- **Phase 6:** Citizen Alerts and Feedback Loop
- **Phase 7:** Reporting and Final Polish

---
*For a more detailed breakdown of the architecture, database design, and APIs, refer to the [Plan.md](./Plan.md).*
