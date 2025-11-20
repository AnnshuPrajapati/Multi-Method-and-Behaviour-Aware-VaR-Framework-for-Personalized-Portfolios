# Multi-Method VaR Framework with Behavioral Finance & Regime Switching

**Advanced portfolio risk management system combining 5 VaR methodologies, behavioral finance, and dynamic market regime detection**


## 🎯 Project Overview

Built a comprehensive risk quantification framework that **outperforms institutional benchmarks by 69%** (Sharpe Ratio: 1.05 vs 0.62) through intelligent integration of quantitative methods and behavioral insights.

### Key Innovations
- **5 VaR Methods**: Historical, Parametric, Monte Carlo, GARCH, Cornish-Fisher
- **Regime Detection**: Automated bull/bear market identification using SPY rolling returns + momentum filters
- **Behavioral Adaptation**: Dynamic risk profiles adjusting to investor psychology (Conservative/Moderate/Aggressive)
- **Crisis Resilience**: Stress testing across COVID-19 (2020) and 2008 Financial Crisis scenarios

## 📊 Performance Results (2015-2024)

| Strategy | Sharpe Ratio | CAGR | Final Value | vs Benchmark |
|----------|-------------|------|-------------|--------------|
| **Aggressive Regime-Switching** | **1.05** | 35.43% | $8.71 | +69% |
| Moderate Regime-Switching | 1.03 | 15.08% | $2.73 | +66% |
| Conservative Regime-Switching | 1.10 | 12.35% | $2.30 | +77% |
| BlackRock 60/40 | 0.78 | 9.05% | $2.38 | Benchmark |
| Vanguard VSMGX | 0.62 | 7.22% | $2.01 | Benchmark |

**Key Achievement**: 40% crypto allocation maintained lower drawdowns (-40.1%) than pure equity (-52.3%) during 2022 market volatility

## 🛠️ Technical Skills Demonstrated

**Programming & Libraries**
- Python: pandas, NumPy, scikit-learn, SciPy
- Financial Analysis: yfinance, arch (GARCH models)
- Visualization: Matplotlib, Seaborn, Plotly
- Machine Learning: Random Forest for ML-based VaR

**Quantitative Finance**
- Value at Risk (VaR) modeling across 5 methodologies
- GARCH volatility modeling for time-varying risk
- Monte Carlo simulation (100,000 paths)
- Backtesting with breach analysis (95% confidence level)

**Financial Engineering**
- Regime-switching portfolio strategies
- Behavioral finance integration (Prospect Theory)
- Transaction cost optimization (0.15% per trade, 30% turnover cap)
- Multi-asset portfolio construction (equities, bonds, crypto, commodities)



## 📁 Repository Contents
```
├── Multi-Method-&-Behavior-Aware-VaR.py    # Complete Python implementation with all VaR methods, regime detection, behavioral models, and backtesting
├── RPM_Research_Paper.pdf                   # Full academic paper with methodology, empirical results, literature review, and appendices
├── Presentation.pdf                         #  Executive presentation with intial findings and visual summaries 
├── Methodology.drawio.png                   # System architecture and data flow diagram 
├── Strategy Diagram Brainstorm.png          # Conceptual framework and strategy logic
└── README.md                                # This file
```

## 🔬 Methodology Highlights

**Market Regime Detection**
- SPY 1-year rolling return + momentum filter
- Reduces false positives by 37% vs single indicators
- Dynamic allocation: 30% defensive shift in bear markets

**Behavior-Weighted VaR Formula**
```
VaR_behavioral = VaR_base × (1 + α)
α = +0.20 (Conservative), 0.00 (Moderate), -0.20 (Aggressive)
```

**Stress Testing Results**
- COVID Crash: -6.85% VaR across all profiles (systemic convergence)
- 2008 Crisis: Conservative -1.63% vs Aggressive -3.5% (behavioral divergence)



## 📈 Business Impact

✅ **42% reduction** in bear market losses through regime-adaptive allocation  
✅ **77% higher** risk-adjusted returns vs traditional 60/40 portfolio  
✅ **89% preservation** of bull market gains during regime transitions  
✅ **17 strategic trades** over 10 years (low turnover = cost efficiency)


## 🔑 Key Features in Code
```python
# 5 VaR Methodologies
- historical_var()          # Empirical distribution
- parametric_var()          # Normal distribution assumption
- monte_carlo_var()         # 100K path simulation
- garch_var_cached()        # Time-varying volatility
- cornish_fisher_var()      # Skewness/kurtosis adjusted

# Regime Detection
- detect_market_regime()    # SPY rolling returns
- momentum_signal()         # Cross-asset momentum
- generate_trade_signal()   # Combined bull/bear signal

# Behavioral Finance
- compute_behavior_weighted_var()    # Psychology-adjusted risk
- simulate_behavioral_stress()       # Crisis response modeling
```

## 💼 Applications

- **Portfolio Management**: Dynamic asset allocation for wealth managers
- **Risk Management**: Enhanced VaR forecasting for financial institutions  
- **Algorithmic Trading**: Regime-based strategy signals
- **Financial Planning**: Personalized risk assessment for advisors


