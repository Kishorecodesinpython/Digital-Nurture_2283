# E-commerce Platform Search Function 🛍️

This project implements the **search functionality** of an e-commerce platform using **C# console application**. It demonstrates how to apply **Linear Search** and **Binary Search** algorithms to search through a product list by product name.

---

## 📌 Features

- `Product` class with attributes: `ProductId`, `ProductName`, and `Category`.
- Implementation of:
  - ✅ **Linear Search**: Suitable for unsorted lists.
  - ✅ **Binary Search**: Fast and efficient for sorted lists.
- Console-based interface for demonstration.

---

# 💰 Financial Forecasting using Recursion (C#)

## 📌 Project Overview
This C# console application forecasts future financial values based on an initial amount, a yearly growth rate, and a forecast duration (in years). The forecasting logic is implemented using **recursion** and can be optimized using **memoization**.

---

## 🧠 How It Works

The recursive formula used:

FutureValue(n) = FutureValue(n-1) * (1 + GrowthRate)


- **Base Case:** If year = 0, return the initial amount.
- **Recursive Case:** Multiply the previous year’s forecast by (1 + rate).

---

## 🧪 Sample Output

Enter the initial amount: 1000
Enter annual growth rate (in %): 5
Enter number of years to forecast: 3

Forecasted value after 3 years: ₹1,157.63


---

## 🚀 Features

- 🧮 Recursive algorithm for future value calculation
- ⚡ Memoization support to optimize performance
- 💬 Interactive user input via console
- 📊 Accurate compound growth simulation

---

## 🛠 Tech Stack

- **Language:** C#
- **Framework:** .NET (Framework/Core/6/7 Compatible)
- **IDE:** Visual Studio / Visual Studio Code

---

## 🧾 Code Snippet

### 🔁 Basic Recursive Version

```csharp
static double ForecastValue(double amount, double rate, int year)
{
    if (year == 0)
        return amount;
    return ForecastValue(amount, rate, year - 1) * (1 + rate / 100);
}

