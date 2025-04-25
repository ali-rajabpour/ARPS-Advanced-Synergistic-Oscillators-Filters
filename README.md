# ARPS Advanced Synergistic Oscillators & Filters
**Originally created: September 07, 2020**
*(Note: This script was created in 2020 but is being shared on GitHub on 2025-04-25)*

---

# ARPS Advanced Synergistic Oscillators & Filters

## Overview

The **ARPS Advanced Synergistic Oscillators & Filters** is a comprehensive and versatile Pine Script indicator designed to enhance trading decision-making by leveraging multiple advanced algorithms and technical indicators. It includes fully customizable implementations of the Stochastic Momentum Index (SMI), Moving Average Convergence Divergence (MACD), Ehlers Stochastic CG Oscillator (ESCGO), and Ehlers Smoothed Stochastic. Additionally, this script supports multiple timeframes and incorporates visuals and alerts for actionable signals.

The script integrates advanced features, such as adaptive roofing filters, multiple configurable inputs, and fine-tuned crossover logic, making it ideal for experienced traders seeking more reliable market insights.

---

## Key Features

### 1. **Stochastic Momentum Index (SMI)**
   
   - Calculation of stochastic values (`SMI`, `SMIsignal`, and `emasignal`).
   - Highlights overbought and oversold zones dynamically.
   - Customizable display options with clear color-coded signals.
   - Two threshold levels (`+40` and `-40`) for decision-making support.
   - Visual crossovers between `SMIsignal` and `emasignal` for detecting trend reversals.

### 2. **Moving Average Convergence Divergence (MACD)**
   
   - Full implementation of MACD with user-defined lengths for fast and slow MAs.
   - Signals for MACD histogram trends:
     - Color-coded patterns for increasing or decreasing positive and negative momentum.
   - Configurable visualization with histogram, signal line, and MACD line.
   - Alerts for strong and weak entry signals based on crossover logic.

### 3. **Ehlers Stochastic CG Oscillator (ESCGO)**
   
   - Combines adaptive cyclic gain logic with stochastic principles.
   - Includes levels (`+0.8` and `-0.8`) to indicate overbought or oversold conditions.
   - Trigger signals when `v2` (oscillator) crosses the trigger line (`t`).
   - Integrated logic for refined long and short entry conditions.
   - Visual fills and plots for easy interpretation of oscillator trends.

### 4. **Ehlers Smoothed Stochastic**
   
   - Based on smoother and more adaptive roofing filter logic.
   - Facilitates noise reduction in identifying trend changes.
   - Customizable parameters:
     - Stochastic length, smoothing MA length, and roofing band upper/lower frequencies.
   - Dynamic alerts based on crossovers between smoothed stochastic and its moving average.

### 5. **Alerts Functionality**
   
   - Alerts for:
     - MACD crossover signals (strong and weak for long/short entries).
     - ESCGO long and short trigger conditions.
     - Ehlers Smoothed Stochastic crossovers.
     - Combined signals between ESCGO and Smoothed Stochastic for enhanced entry points.
   - Configurable messages for alert notifications in trading platforms.

### 6. **Customizability**
   
   - Enable or disable specific indicators (`ShowSMI`, `ShowMACD`, `ShowESCGO`, `ShowESS`).
   - Configurable input settings for every module, allowing users to fine-tune the script based on their trading style.
   - Adjustable timeframe compatibility.

---

## Script Parameters

### Stochastic Momentum Index (SMI)
   - `Percent K Length`: Moving average window size for percent K calculation (default: 10).
   - `Percent D Length`: EMA smoothing length (default: 3).
   - `Overbought` and `Oversold` levels: Custom thresholds for identifying extremes (default: ±40).

### Moving Average Convergence Divergence (MACD)
   - `Fast Length`: Length for the fast-moving average (default: 12).
   - `Slow Length`: Length for the slow-moving average (default: 26).
   - `Signal Length`: Smoothing applied to MACD (default: 9).
   - `Show MacD & Signal Line`: Toggles the display of MACD and Signal Line.
   - `Histogram Settings`: Histogram color customization and visibility options.

### Ehlers Stochastic CG Oscillator (ESCGO)
   - `Oscillator Length`: Length determining dynamic oscillator window (default: 8).
   - OB/OS Level: ±0.8 threshold for overbought/oversold regions.

### Ehlers Smoothed Stochastic
   - `Stoch Length`: Length used for stochastic calculation (default: 14).
   - `Stoch MA Length`: Moving average length for stochastic smoothing (default: 3).
   - `Roofing Bands`: Upper (48) and lower (10) frequency bounds for adaptive smoothing.

---

## Alerts

This script includes customizable alerts to notify you when critical trading conditions are met:

1. **MACD Alerts**
   - Strong or weak long/short entries based on MACD crossovers and histogram relations.

2. **ESCGO Alerts**
   - Long/short entry conditions based on CG oscillator momentum shifts.

3. **Ehlers Smoothed Stochastic Alerts**
   - Crossovers between stochastic values and their moving averages.

4. **Combination Alerts**
   - Synergistic long/short entries when both ESCGO and Smoothed Stochastic align.

---

## Usage

1. Copy and paste the script into Pine Script Editor in TradingView.
2. Adjust the input parameters according to your trading strategy.
3. Apply the script to your desired chart.
4. Enable alert conditions for automatic notifications.

---

## Visualizations

This script provides a clear visual interface, including:
   - Overbought/oversold areas shaded in the chart.
   - Trend-specific coloring for lines and histogram bars.
   - Cross-style markers at critical crossover points.

---

## Disclaimer

This script is a technical analysis tool and should be used as part of a broader trading strategy. It is not intended as financial advice, and the author is not responsible for any trading losses incurred.

---

By: **Ali Rajabpour Sanati**
Email: [ali.poursanati@gmail.com](mailto:ali.poursanati@gmail.com)