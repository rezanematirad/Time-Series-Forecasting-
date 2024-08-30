# Time Series Forecasting Project

## Overview

This project aims to apply advanced machine and deep learning models to time series forecasting. Various learning models including, **LSTM**, **BiLSTM**, **ConvLSTM**, **GRU**, **LightGBM**, **RandomForest**, **ResLSTM**, **RNN**, and **XGBoost** are developed. To have a fair and comprehensive analysis of performance, the models are tested on standard time series data including **Electricity Transformer Temperature (ETT)**, **Electricity load demand**, **Traffic**, **weather**, and **finance** datasets.

## Table of Contents
- [Project Structure](#project-structure)
- [Data](#data)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Data
These datasets are commonly used for benchmarking time series forecasting models in academic research and competitions, covering domains like temperature, electricity, transportation, weather, and health. See the table below for details.

| Dataset      | Number of columns | Prediction Horizon  | Train/Validation/Test Size | Frequency | Domain       |
|--------------|-------------------|---------------------|----------------------------|-----------|--------------|
| ETTm1        | 7                 | {96, 192, 336, 720} | (34465, 11521, 11521)      | 15 min    | Electricity Transformer Temperature  |
| ETTm2        | 7                 | {96, 192, 336, 720} | (34465, 11521, 11521)      | 15 min    | Electricity Transformer Temperature  |
| ETTh1        | 7                 | {96, 192, 336, 720} | (8545, 2881, 2881)         | 1 hour    | Electricity Transformer Temperature  |
| ETTh2        | 7                 | {96, 192, 336, 720} | (8545, 2881, 2881)         | 1 hour    | Electricity Transformer Temperature  |
| Electricity  | 321               | {96, 192, 336, 720} | (18317, 2633, 5261)        | 1 hour    | Electricity Load Demand  |
| Traffic      | 862               | {96, 192, 336, 720} | (12185, 1757, 3509)        | 1 hour    | Transportation|
| Weather      | 21                | {96, 192, 336, 720} | (36792, 5271, 10540)       | 10 min    | Weather      |
| ILI          | 7                 | {24, 36, 48, 60}    | (617, 74, 170)             | 1 week    | Illness      |

## Installation

To set up the environment and install the required packages, follow these steps:

1. **Clone the Repository:**

   First, clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/time-series-forecasting.git
   cd time-series-forecasting
   ```

2. **Install Required Packages:**

   It is recommended to create your own virtual environment and install the necessary packages as follows:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

## Usage

To run the models, navigate to the `scripts` folder, pick the intended `.sh` file, and execute it using the following commands:

```bash
sh ./scripts/Bilstm.sh
sh ./scripts/Conv2DLSTM.sh
sh ./scripts/RandomForest.sh
sh ./scripts/RNN.sh
```

## Acknowledgements

This project makes use of code from the following open-source projects:

- **[TimesNet]([https://github.com/thuml/TimesNet](https://github.com/thuml/Time-Series-Library))** - A deep learning model for time series forecasting developed by THUML @ Tsinghua University, used under the MIT License.

We are grateful to the authors for their contributions to the open-source community.
