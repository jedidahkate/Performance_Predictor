# Performance_Predictor
System design for ranking of companies based on market trends and company relationships
# Relationship-Aware Market Performance Prediction System

## Goal
The goal of this system is to analyze historical market behavior and relationships between companies in order to predict which companies are likely to perform better than others on the next trading day.

The focus is on relative performance rather than exact price prediction.

## Design Approach
The system processes historical market data such as returns, volume, and volatility across multiple companies. To handle variability across sectors and company sizes, indicators are normalized within sectors.

Rolling historical windows are used to capture short-term and medium-term trends while allowing the system to adapt to changing market conditions.

## Inter-Company Relationships
Relationships between companies are identified using:
- Rolling correlation of returns
- Sector and industry grouping
- Consistent co-movement patterns

These relationships are updated continuously so that evolving market dynamics are reflected in the analysis.

## Interpretability
The system avoids black-box models. Each company’s score is derived from:
- Individual performance trends
- Influence from related companies or sector peers

This makes predictions explainable and justifiable using observable historical data.

## Expected Output
- A score or ranking for each company indicating expected performance relative to others
- Clear signals highlighting stronger or weaker expected performers
- Optional insights showing which company interactions contributed most to the final score

## Outcome
The system provides actionable, easy-to-understand insights that support decision-making without relying on overly complex modeling techniques.
