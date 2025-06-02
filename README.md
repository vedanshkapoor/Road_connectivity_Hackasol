# 🛣️ Road Network Connectivity Prediction using Geospatial Data & Machine Learning

This project aims to **analyze and predict road network connectivity** using a combination of **machine learning**, **graph algorithms**, and **geospatial data**, enhanced with APIs for distance and elevation. The region of focus is **Chamoli district, Uttarakhand, India**.

---

## 📌 Project Overview

We build an intelligent pipeline that integrates:
- Road network data from **OpenStreetMap (OSM)**
- Elevation data from **Google Elevation API**
- Distance data from **Google Distance Matrix API**
- **Slope** and **curvature** calculations
- **Floyd-Warshall algorithm** for shortest path analysis

We are also actively working on extending this using **Graph Neural Networks (GNNs)** for spatial inference.

---

## 🚀 Key Features

| Feature                     | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| 🗺️ Road Network Loading     | Load and visualize road networks using OSMnx for Chamoli district.          |
| ⛰️ Altitude Fetching        | Fetch elevation data using **Google Elevation API**.                        |
| 📏 Distance Calculation     | Compute real-world distances via **Google Distance Matrix API**.           |
| 📐 Slope Estimation         | Calculate slope based on elevation and distance between nodes.             |
| 🌀 Curvature Calculation    | Estimate road curvature using **Shapely** geometric properties.            |
| 🔀 Shortest Path Analysis   | Apply **Floyd-Warshall algorithm** considering slope as the edge weight.   |
| 📊 Visualization            | Render the road network graph without cluttering edge weights.             |
| 🤖 GNN Integration          | Ongoing work using **Graph Neural Networks** for predictive modeling.      |

---

## 🧰 Tech Stack

### ⚙️ Languages & Environment
- **Python 3.x**
- IDE: *PyCharm* (recommended)
- OS: *Windows / Linux* (project tested on both)

### 📦 Python Libraries
| Library      | Purpose                                        |
|--------------|------------------------------------------------|
| `osmnx`      | Download and visualize road networks           |
| `networkx`   | Graph construction and analysis                |
| `pandas`     | Data manipulation                              |
| `matplotlib` | Graphical visualizations                       |
| `requests`   | API calls to external services                 |
| `shapely`    | Geometric calculations                         |

### 🌐 APIs Used
- **Google Maps Elevation API**
- **Google Maps Distance Matrix API**

### 📊 Algorithm
- **Floyd-Warshall** for shortest path based on slope-weighted edges.

---

## 🗂️ Data Sources

| Source                   | Description                                |
|--------------------------|--------------------------------------------|
| OpenStreetMap (OSM)      | Primary road network data                  |
| Google Earth             | Visual reference and mapping               |
| NASA Earthdata (SRTM)    | Digital Elevation Model (DEM) data         |
| GPS Visualizer           | Coordinate referencing                     |
| QGIS                     | Spatial data analysis                      |
| Custom CSV Input         | Latitude & longitude coordinate mappings   |

---

## 📈 Results

### ✅ Feasibility Analysis

We evaluated new node connections based on slope and distance constraints:

| Criteria                         | Result                                   |
|----------------------------------|------------------------------------------|
| Feasibility Threshold (Distance) | 20 km                                    |
| Evaluation District              | Chamoli, Uttarakhand                     |
| Connectivity Status              | Generated feasible/non-feasible matrix   |

### 🌍 SRTM-DEM Dataset

- Created a dataset combining **Digital Elevation Model** (DEM) data across **Uttarakhand**.
- Incorporated into road analysis for improved accuracy.

### 📋 Road Network Report

- Generated an infrastructure report highlighting:
  - Areas with high slope or curvature (challenging terrain)
  - Gaps in connectivity
  - Opportunities for road expansion or rerouting

---

## 🧠 GNN Integration (Ongoing)

We are currently implementing **Graph Neural Networks** (GNNs) to:
- Predict future road expansion zones
- Identify optimal road construction plans
- Learn spatial patterns in road feasibility and elevation dynamics

---

## 📁 Project Structure

