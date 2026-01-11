# Quick Start Guide

## Installation

```bash
npm install
```

## Running the Application

```bash
npm start
```

The application will open at `http://localhost:3000`

## Features Overview

### Dashboard
- View current period usage and metrics
- See Usage DNA classification
- View Silent Damage Score
- Receive personalized suggestions
- Conditional awareness videos for risky patterns

### Add Data
- Enter daily usage manually
- Add optional notes for context
- View recent entries
- See real-time recommendations

### Analytics
- Predictive limit breach forecasts
- 14-day usage predictions
- Scenario simulations with different reduction levels
- Detailed pattern analysis with explanations
- Transparent methodology display

## Data Storage

Currently uses localStorage. To enable Firebase:

1. Create a Firebase project at https://console.firebase.google.com
2. Copy `src/firebase/config.example.js` to `src/firebase/config.js`
3. Add your Firebase credentials
4. Update storage utilities to use Firebase instead of localStorage

## Key Algorithms

### Pattern Analysis
- **Rolling Average**: 7-day moving average for smoothing
- **Trend Detection**: Linear regression for direction and strength
- **Anomaly Detection**: Statistical Z-score analysis (2σ threshold)
- **Adaptive Baseline**: Exponential moving average (α=0.1)

### Predictive Analytics
- **Limit Breach Prediction**: Projects usage based on current rate and trends
- **Future Usage Forecast**: 30-day linear projection
- **Scenario Simulation**: Models different reduction scenarios

### Usage DNA Classification
Profiles: Efficient, Moderate, High-Consumer, Volatile, Improving
- Based on efficiency ratio, consistency, trend direction, and anomaly rate

### Silent Damage Score (0-100)
Components:
- Consumption (0-40): Relative to monthly limit
- Trend (0-25): Penalizes increasing trends
- Consistency (0-20): Penalizes high variance
- Efficiency (0-15): Deviation from baseline

## Color Palette

- **Black**: #000000 - Primary text, buttons
- **White**: #FFFFFF - Background
- **Green**: #00FF88 - Accents, positive indicators

## Project Structure

```
src/
├── components/      # React UI components
├── data/           # Firebase-ready data models
├── firebase/       # Firebase configuration (optional)
├── styles/         # CSS styling
└── utils/          # Core algorithms and utilities
```

## Next Steps for Hackathon

1. **Add Real Video Content**: Replace video placeholders with educational content
2. **Firebase Integration**: Connect to Firebase for persistence
3. **User Authentication**: Add Firebase Auth for multi-user support
4. **Mobile Responsiveness**: Enhance mobile experience
5. **Export Functionality**: Allow users to export their data/reports
6. **Sharing Features**: Enable users to share their Usage DNA profile
