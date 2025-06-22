# 🎮 Loyalty Points Analysis for Real-Money Gaming Platform

This project analyzes user activity on a real-money gaming platform to design and evaluate a **loyalty points system**. The goal is to fairly reward active users based on their deposits, withdrawals, and gameplay patterns, and to ensure accurate and transparent distribution of bonus rewards.

---

## 📊 Problem Statement

A gaming platform wants to identify and reward its most loyal users. The task involves:

- Calculating **loyalty points** for each user based on their activities.
- Dividing each day into two time slots:  
  - **Slot 1 (S1)**: 12:00 AM – 12:00 PM  
  - **Slot 2 (S2)**: 12:00 PM – 12:00 AM
- Identifying the **top 50 users** in each slot and distributing a ₹50,000 bonus fairly among them.
- Evaluating the effectiveness of the loyalty formula and suggesting improvements.

---

## 📁 Dataset Description

The analysis is based on three datasets:

1. **Games Played**
   - `User ID`
   - `Datetime` of gameplay

2. **Deposits**
   - `User ID`
   - `Amount` deposited
   - `Datetime`

3. **Withdrawals**
   - `User ID`
   - `Amount` withdrawn
   - `Datetime`

All timestamps are in IST.

---

## 🧮 Loyalty Points Formula

The loyalty points for each user in each time slot are calculated using the formula:

Loyalty Points = (0.01 * Deposit Amount)
+ (0.005 * Withdrawal Amount)
+ (0.001 * max(Deposits Count - Withdrawals Count, 0))
+ (0.2 * Number of Games Played)


---

## 🛠️ Tools Used

- **Python 3.11**
- **Jupyter Notebook**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn** (for optional visualizations)

---

## 📌 Key Outcomes

- Generated loyalty points for all users per time slot.
- Identified **top 50 users** for both S1 and S2 slots.
- Distributed the ₹50,000 bonus pool proportionally based on loyalty points.
- Suggested improvements to the scoring formula to balance different user behaviors.

---


