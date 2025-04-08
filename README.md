# Dynamic-Portfolio-Allocation-Using-Reinforcement-Learning-

# 🚀 RL-Based Cryptocurrency Portfolio Optimization

A reinforcement learning (RL) framework for **optimal portfolio allocation** in the **cryptocurrency market**. This project leverages **Deep Q-Learning (DQL)** and **Proximal Policy Optimization (PPO)** to automate and optimize the allocation of funds among a set of cryptocurrencies, aiming to maximize returns while minimizing risks.

---

## 📌 Problem Statement

Portfolio allocation in cryptocurrencies involves deciding how to distribute capital across various digital assets to achieve maximum returns with minimal risk. Unlike traditional approaches, this project proposes an RL-based system that **learns directly from market data** and **adapts dynamically** to market changes.

---

## 🧠 Methodology

We implement and compare two reinforcement learning strategies:

- **Deep Q-Network (DQN)**
- **Proximal Policy Optimization (PPO)**

### Key Components:
- **State Space**: Technical indicators and historical prices of selected cryptocurrencies.
- **Action Space**: Portfolio weight allocations for each asset.
- **Reward Function**: Based on portfolio return and risk metrics.
- **Environment**: Simulated cryptocurrency market using historical data.

---

## 📅 Dataset

The dataset consists of historical daily price data for **15 major cryptocurrencies**, including:


Each row in the dataset is indexed by the `Date`, which allows for time-series modeling and portfolio rebalancing based on historical trends.

Example:

| Date       | BTC  | ETH  | ADA  | ... |
|------------|------|------|------|-----|
| 2020-01-01 | 7200 | 130  | 0.03 | ... |
| 2020-01-02 | 7350 | 135  | 0.032| ... |
| ...        | ...  | ...  | ...  | ... |

📁 Data is located in the `data/` directory.

---

## 🧪 Evaluate Algorithms and Models

The RL-based portfolio optimization process consists of the following core stages:

### 1. Creating Environment
- Custom environment simulating a cryptocurrency trading scenario using historical data.

### 2. Helper Functions
- Data preprocessing
- Portfolio return calculation
- Performance metric computation (Sharpe Ratio, Alpha, Beta, Volatility)

### 3. Training Agents
- Train DQN and PPO agents on the custom environment.
- Track performance, rewards, and portfolio evolution during training.

Evaluation plots and performance summaries can be seen in output.

---

## 📊 Results

| Metric        | RL Model (DQN/PPO) | Equal-Weight Benchmark |
|---------------|--------------------|-------------------------|
| Sharpe Ratio  | **0.4044**         | -0.5016                 |
| Volatility    | **0.0184**         | 0.0468                  |
| Alpha         | **0.0001**         | 0                       |
| Beta          | **-0.2758**        | 1.0                     |

✅ **Significantly better risk-adjusted returns**  
✅ **Reduced volatility and market exposure**

---

## 🛠️ Tech Stack

- **Programming Language**: Python
- **Data Handling**:  
  - `pandas` – Data manipulation and preprocessing  
  - `numpy` – Numerical operations  
- **Data Visualization**:  
  - `matplotlib` and `seaborn` – Plotting and analysis  
- **Machine Learning / Deep Learning**:  
  - `scikit-learn` – Standardization and scaling  
  - `Keras` (with TensorFlow backend) – Neural network implementation  
- **Reinforcement Learning**:  
  - Custom DQN logic using `deque`, `random`, and `numpy.random.choice`  
- **Utility**:  
  - `datetime` – Date and time management  
  - `math` – Mathematical operations  

---




