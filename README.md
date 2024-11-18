# Capture-Mark-Recapture Estimators: Shiny Application

This repository contains a Shiny application for exploring **Capture-Mark-Recapture (CMR) Estimators**, designed for use in the **Population Ecology** course in the Biology program at **Ghent University (UGhent)**.

The app provides tools to simulate and estimate population parameters using two different CMR approaches:  
1. **Jolly-Seber Estimator** (for open populations)  
2. **Petersen Estimator** (for closed populations)

---

## Features

### 1. Jolly-Seber Estimator
- Simulate capture histories for populations with **births** and **deaths** between capture sessions.
- View detailed metrics for each capture session:
  - Total captures (`n`)
  - Unmarked individuals (`u`)
  - Marked individuals (`m`)
  - Recaptured individuals (`r`)
  - Marked-but-missed individuals (`z`)
  - Population estimates (`M`, `N`, `Φ`, `B`)
- Visualize capture histories in an interactive and sortable table.

### 2. Petersen Estimator
- Simulate recaptures for **closed populations** using user-defined parameters:
  - Actual population size
  - Number of marked individuals
  - Sample size in second capture
- Automatically calculate:
  - Estimated population size (`N̂`)
  - Standard error of the estimate (`SE`)

### General Features
- **Interactive UI**: Adjust input parameters to see results in real-time.
- **Error Handling**: Receive notifications for invalid parameter inputs (e.g., marked individuals exceeding population size).
- **Educational Focus**: Designed to teach fundamental concepts of population estimation and the challenges of sampling wildlife populations.

---

## Installation Instructions

### Prerequisites
Make sure you have the following installed on your computer:
- R (version 4.0 or higher)
- RStudio (optional, for development purposes)

### Required R Packages
The app requires the following R packages:  
- `shiny`: For building the interactive web application  
- `DT`: For displaying interactive data tables  

The app automatically checks for and installs missing packages when run.

---

## Input Parameters

### Jolly-Seber Estimator
- **Initial Population Size**: The size of the population at the start of the simulation.
- **Number of Captures per Event**: The number of individuals captured in each session.
- **Births (Influx)**: The number of new individuals entering the population between sessions.
- **Deaths (Outflow)**: The number of individuals leaving the population between sessions.

### Petersen Estimator
- **Population Size**: The actual population size (used to simulate results).
- **Marked Individuals**: The number of individuals marked during the first capture.
- **Sample Size in Second Capture**: The number of individuals captured in the second session.

---

## Outputs

### Jolly-Seber Results
- **Simulation Results Table**: Displays key metrics for each session.
- **Capture Histories Table**: Provides a detailed capture matrix for sorting and filtering.

### Petersen Results
- **Results Table**: Displays the population size estimate (`N̂`) and its standard error.

---

## Educational Context

This application was developed as a teaching tool for the **Population Ecology** course in the **Biology Department at Ghent University (UGhent)**. It allows students to:
- Understand the principles and assumptions of CMR methods.
- Explore the effects of demographic processes on population estimates.
- Practice data interpretation and parameter estimation in ecological studies.

---

## Contributions

Contributions are welcome to improve this educational tool. If you would like to contribute, please fork the repository, make your changes, and submit a pull request.

---


For questions or feedback, feel free to reach out to **Bram Vanden Broecke** or the **Population Ecology course team** at Ghent University.
