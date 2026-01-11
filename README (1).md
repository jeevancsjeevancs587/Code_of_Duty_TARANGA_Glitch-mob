# Voltrix

A hackathon-winning web application that helps users become aware of their resource usage through behavioral pattern analysis, predictive analytics, and personalized reduction strategies.

## Features

- **Pattern Analysis**: Rolling averages, trend detection, anomaly detection, self-updating baselines
- **Predictive Analytics**: Forecasts when users will exceed limits and simulates future outcomes
- **Usage DNA**: Classifies users into behavioral profiles
- **Silent Damage Score**: Represents hidden long-term environmental impact
- **Personalized Suggestions**: Data-driven micro-suggestions for reducing usage
- **Educational Videos**: Conditionally triggered educational content

## Tech Stack

- React 18
- Firebase (ready for integration)
- Recharts for visualizations
- Date-fns for date handling

## Getting Started

```bash
npm install
npm start
```

## Architecture

- `/src/utils` - Pattern analysis algorithms and analytics
- `/src/components` - React UI components
- `/src/data` - Firebase-ready data models
- `/src/styles` - Global styles and theme

## Color Palette

- Black (#000000)
- White (#FFFFFF)
- Green (#00FF88)
