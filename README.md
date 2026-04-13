# Stock AI Agent RL S&P

An automated trading system utilizing **Reinforcement Learning** to navigate the top 10 assets of the S&P 500. This project leverages the **FinRL** framework to bridge the gap between financial data and deep learning models.

## Project Goal
The objective is to train and compare different RL agents to optimize portfolio returns using the most liquid and influential stocks in the market.

## Universe of Stocks
The agent trades the following tickers:
`['AAPL', 'MSFT', 'NVDA', 'AMZN', 'GOOGL', 'META', 'TSLA', 'BRK-B', 'WMT', 'JPM']`

## Core Technologies
* **Environment:** [FinRL](https://github.com/AI4Finance-Foundation/FinRL) (built on OpenAI Gym/Gymnasium).
* **Algorithms:** 
    * **PPO:** Proximal Policy Optimization
    * **A2C:** Advantage Actor-Critic
    * **DDPG:** Deep Deterministic Policy Gradient
* **Data Source:** Yahoo Finance / Alpaca via FinRL integration.


### Team & Responsibilities

The following table outlines the distribution of work for implementing the specific Reinforcement Learning models:

| Algorithm | Team Member |
| :--- | :--- |
| **A2C** (Advantage Actor-Critic) | Radek Szewczyk |
| **DDPG** (Deep Deterministic Policy Gradient) | Jan Zubalewicz |
| **PPO** (Proximal Policy Optimization) | Mateusz Kubita |

### Dataset Configuration

To ensure consistent results across all models, we have defined the following timelines for training and backtesting:

| Period | Start Date | End Date |
| :--- | :--- | :--- |
| **Training Range** | `2018-01-01` | `2023-01-01` |
| **Trading / Testing Range** | `2023-01-01` | `2024-01-01` |

**Constants used in the code:**
```python
TRAIN_START_DATE = '2018-01-01'
TRAIN_END_DATE = '2023-01-01'
TRADE_START_DATE = '2023-01-01'
TRADE_END_DATE = '2024-01-01'

