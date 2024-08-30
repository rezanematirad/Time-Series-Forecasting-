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
These datasets are commonly used for benchmarking time series forecasting models in academic research and competitions like like temperature, electricity, transportation, weather, and health. See the table below for details.

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

