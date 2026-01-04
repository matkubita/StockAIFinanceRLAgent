# Stock AI Agent RL S&P

An automated trading system utilizing **Reinforcement Learning** to navigate the top 10 assets of the S&P 500. This project leverages the **FinRL** framework to bridge the gap between financial data and deep learning models.

## 🚀 Project Goal
The objective is to train and compare different RL agents to optimize portfolio returns using the most liquid and influential stocks in the market.

## 📊 Universe of Stocks
The agent trades the following tickers:
`['AAPL', 'MSFT', 'NVDA', 'AMZN', 'GOOGL', 'META', 'BRK.B', 'TSLA', 'AVGO', 'JPM']`

## 🧠 Core Technologies
* **Environment:** [FinRL](https://github.com/AI4Finance-Foundation/FinRL) (built on OpenAI Gym/Gymnasium).
* **Algorithms:** * **PPO:** Proximal Policy Optimization
    * **A2C:** Advantage Actor-Critic
    * **DDPG:** Deep Deterministic Policy Gradient
* **Data Source:** Yahoo Finance / Alpaca via FinRL integration.


### 👥 Team & Responsibilities

The following table outlines the distribution of work for implementing the specific Reinforcement Learning models:

| Algorithm | Team Member |
| :--- | :--- |
| **PPO** (Proximal Policy Optimization) | Mateusz Kubita |
| **A2C** (Advantage Actor-Critic) | Radek Szewczyk |
| **DDPG** (Deep Deterministic Policy Gradient) | Jan Zubalewicz |

