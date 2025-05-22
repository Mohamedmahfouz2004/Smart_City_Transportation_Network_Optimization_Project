# Smart City Transportation Project

## Overview
This project implements a comprehensive transportation network simulation and optimization system for smart cities. It includes various algorithms for route planning, traffic management, and public transportation optimization.

## Project Structure
```
smart_city_transportation/
├── algorithms/
│   ├── dynamic_programming/
│   │   └── dp_solutions.py
│   ├── greedy/
│   │   ├── a_star.py
│   │   └── dijkstra.py
│   ├── mst/
│   │   └── modified_mst.py
│   └── transit/
│       └── transit_integration.py
├── data/
│   └── excel/
│       ├── Current Bus Routes.xlsx
│       ├── Current Metro Lines.xlsx
│       ├── Existing Roads.xlsx
│       ├── Important Facilities.xlsx
│       ├── Neighborhoods and Districts.xlsx
│       ├── Potential New Roads.xlsx
│       ├── Public Transportation Demand.xlsx
│       └── Traffic Flow Patterns.xlsx
├── docs/
│   ├── gap_analysis.md
│   └── technical_report.md
├── src/
│   └── utils/
│       ├── data_loader.py
│       └── graph_utils.py
└── app.py
```

## Features
- **Multi-modal Transportation**: Simulate routes using cars, buses, metro, or emergency vehicles
- **Traffic-aware Routing**: Consider traffic conditions at different times of day
- **Emergency Vehicle Simulation**: Simulate the impact of emergency vehicles on regular traffic
- **Network Analysis**: View and analyze the transportation network graph

## Algorithms
The project implements several algorithms for transportation network optimization:

### Greedy Algorithms
- **Dijkstra's Algorithm**: For finding shortest paths with traffic considerations
- **A* Algorithm**: For emergency vehicle routing with heuristic optimization

### Dynamic Programming Solutions
- **Schedule Optimization**: For optimizing public transportation schedules
- **Resource Allocation**: For road maintenance with budget constraints
- **Memoized Path Planning**: For improving performance of route planning algorithms

### Minimum Spanning Tree (MST) Algorithms
- **Budget-constrained MST**: For network planning with budget constraints
- **Connectivity-based MST**: For prioritizing connections between important facilities

### Transit Integration Algorithms
- **Multi-modal Path Planning**: For finding optimal paths using multiple transportation modes
- **Transit Connection Optimization**: For improving connections between different transit modes
- **Bus Route Optimization**: For optimizing bus routes based on demand and population distribution

## Data Files
The project uses several Excel files for data input:
- **Current Bus Routes.xlsx**: Information about existing bus routes
- **Current Metro Lines.xlsx**: Information about existing metro lines
- **Existing Roads.xlsx**: Information about existing roads
- **Important Facilities.xlsx**: Information about important facilities (hospitals, schools, etc.)
- **Neighborhoods and Districts.xlsx**: Information about neighborhoods and districts
- **Potential New Roads.xlsx**: Information about potential new roads
- **Public Transportation Demand.xlsx**: Information about public transportation demand
- **Traffic Flow Patterns.xlsx**: Information about traffic flow patterns at different times of day

## Usage
1. Ensure all data files are in the `data/excel/` directory
2. Run the application with Streamlit:
   ```
   streamlit run app.py
   ```
3. Use the web interface to simulate transportation routes and analyze the network

## Requirements
- Python 3.8+
- Streamlit
- NetworkX
- Pandas
- Folium
- Matplotlib
- NumPy

## Installation
```
pip install streamlit networkx pandas folium matplotlib numpy streamlit-folium streamlit-option-menu
```
