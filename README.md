# Week 5 Dashboard Class Activity

## Campus Pulse Dashboard

This project is a Streamlit dashboard built for the Week 5 Dashboard Class Activity. The dashboard presents a mock smart campus operations centre called **Campus Pulse**, showing resource usage, occupancy, and environmental impact across several campus buildings.

The dashboard uses generated dummy data to simulate hourly campus readings for:

* Electricity usage
* Water usage
* WiFi users
* Attendance
* CO2 emissions

## Features

* KPI metric cards with hourly percentage changes
* 24-hour sparkline trends
* Interactive Altair visualisations
* Building-level electricity comparison
* Click-to-filter interaction for building data
* Composite chart showing electricity demand and CO2 emissions
* Current building load comparison between WiFi users and attendance
* Design notes section explaining dashboard choices
* Refresh button to regenerate mock data

## Technologies Used

This project was built with:

```txt
streamlit>=1.18.0
pandas>=2.0.0
altair>=5.2.0
```

## File Structure

```txt
.
├── dashboard.py
└── README.md
```

## Installation

Install the required Python packages using pip:

```bash
pip install streamlit pandas altair
```

Alternatively, if you have a `requirements.txt` file, install the dependencies using:

```bash
pip install -r requirements.txt
```

## How to Run

From the project folder, run the Streamlit application with:

```bash
streamlit run .\dashboard.py
```

On macOS or Linux, you can use:

```bash
streamlit run dashboard.py
```

## Dashboard Overview

The dashboard contains two main views:

### 1. Overview

The Overview page displays the main campus dashboard. It includes KPI cards, trend charts, building comparison charts, and occupancy visualisations.

Users can click on a building bar to filter the main energy and CO2 chart by that building. Clicking outside the bars resets the view back to the whole-campus overview.

### 2. Design Notes

The Design Notes page explains the dashboard design decisions, including:

* Why KPI cards are used
* Why sparklines are useful
* How the composite chart works
* How click interaction improves analysis
* How annotations can highlight important events
* How a real-time update strategy could work in a production system

## Data Source

The dashboard uses mock data generated directly inside the Python script. The data is created using a function that simulates hourly readings for five campus buildings:

* Engineering
* Library
* Science
* Student Centre
* Administration

The generated data is not from a real campus system. It is intended for learning, demonstration, and dashboard design practice.

## Purpose of the Activity

The purpose of this class activity is to practise building an interactive dashboard using Streamlit, pandas, and Altair. It demonstrates how data can be presented using suitable chart types, dashboard layout, visual hierarchy, and interaction techniques.

## Notes

This dashboard is designed as a prototype. In a real-world implementation, the mock data could be replaced with live data from IoT sensors, access systems, electricity meters, water meters, or campus APIs.
