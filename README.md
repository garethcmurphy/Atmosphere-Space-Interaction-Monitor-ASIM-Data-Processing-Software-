# Atmosphere-Space Interaction Monitor (ASIM) Data Processing Software

**A Python-based software suite for processing and analyzing data from the Atmosphere-Space Interaction Monitor (ASIM) onboard the International Space Station (ISS).**

---

## Overview

The Atmosphere-Space Interaction Monitor (ASIM) is a scientific payload aboard the ISS, designed to observe and study high-energy phenomena in Earth's upper atmosphere, such as:

- **Transient Luminous Events (TLEs):** Sprites, Blue Jets, and Elves.
- **Terrestrial Gamma-ray Flashes (TGFs).**

This Python software processes raw telemetry data from ASIM, converting it into actionable insights for researchers. It enables automated data ingestion, calibration, event detection, and visualization of atmospheric phenomena.

---

## Key Features

1. **Telemetry Parsing**:
   - Processes raw data streams from the ISS.
   - Implements telemetry data models for structured parsing.

2. **Data Calibration**:
   - Corrects for instrumental biases.
   - Applies geometric and energy calibration for scientific accuracy.

3. **Event Detection**:
   - Identifies TLEs and TGFs using pattern recognition algorithms.
   - Logs detected events with timestamped metadata.

4. **Data Visualization**:
   - Generates time-series plots, spectrograms, and event-specific overlays.
   - Interactive tools for exploring event datasets.

5. **Django Integration**:
   - Provides a web interface for managing telemetry datasets.
   - Supports metadata queries and real-time event dashboards.

6. **Modular Architecture**:
   - Extensible design allows integration of custom processing pipelines or algorithms.

---

## Getting Started

### Prerequisites

Ensure the following are installed:

- Python 3.8 or later.
- Common Python libraries like NumPy, Pandas, Matplotlib, and SciPy.
- Optional libraries for advanced functionality, such as Astropy or H5py.

---

### Installation

1. Clone the repository and navigate to the project folder.
2. Install dependencies using `pip` or a dependency manager like Poetry.
3. Ensure required input data is available in the specified directories.

---

### Usage Workflow

1. **Process Raw Telemetry**: Convert raw telemetry data into structured formats for analysis.
2. **Calibrate Data**: Apply calibration algorithms to ensure scientific accuracy.
3. **Event Detection**: Identify and log atmospheric events such as TLEs and TGFs.
4. **Visualize Results**: Create plots and overlays to explore the detected events.

---

## File Structure

```plaintext
asim-data-processing/
├── data/                  # Input and output data directories
├── src/                   # Source code
│   ├── telemetry/         # Telemetry parsing modules
│   ├── calibration/       # Calibration algorithms
│   ├── detection/         # Event detection logic
│   ├── visualization/     # Visualization tools
│   └── web/               # Django app for web interface
├── tests/                 # Unit tests for all modules
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
