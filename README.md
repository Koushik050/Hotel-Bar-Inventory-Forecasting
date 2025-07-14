
# 🍷 Hotel Bar Inventory Forecasting & Reorder Recommendation System

### 📌 Project Overview

This project solves a real-world problem faced by hotel chains that run multiple bar locations. These bars often deal with two major issues — running out of popular drink items (stockouts) and ordering too much of low-demand ones (overstocking). Both of these cause increased costs and unhappy guests.

Using historical inventory data, this project forecasts item-level demand and recommends how much stock should be kept (par level) and when to reorder.

---

### 🎯 Business Problem

- Frequent **stockouts** of high-demand drinks lead to poor guest experience.
- **Overstocking** slow-moving items increases wastage and costs.
- Managers need a **data-driven system** to make smart inventory decisions.

---

### 🛠️ What This Project Does

1. Cleans and processes raw bar inventory data from multiple hotel locations.
2. Calculates daily consumption for each item using:
```

Consumed = Opening + Purchase - Closing

```
3. Forecasts next 7 days' demand using **Holt-Winters Exponential Smoothing**.
4. Calculates the **par level** using:
```

Par Level = (Average Daily Forecast × Lead Time) + Safety Stock (20%)

```
5. Compares with current stock and recommends:
- Whether reorder is needed
- How much to reorder

---

### 🧠 Why Holt-Winters Model?

- Simple and works well for **time-based demand**
- Handles **trends and seasonality** in consumption
- Fast and accurate for short-term forecasting

---

### 📊 Outputs

- Forecasted daily consumption for each Bar + Brand
- Par level per item
- Reorder recommendation (Yes/No)
- Suggested reorder quantity
- Final report exported as Excel (`Inventory_Recommendations.xlsx`)

---

### 🧪 Tools & Technologies

- Python (Pandas, NumPy, Statsmodels, Matplotlib)
- Jupyter Notebook
- Excel/CSV for data input & output
- Time Series Forecasting

---

### 🏪 How This Works in a Real Hotel

The system can run daily or weekly. Each bar manager gets a simple report showing:
- What to reorder
- How much to reorder
- Stock level suggestions (par level)

This avoids both stockouts and overstocking, saving cost and improving guest satisfaction.

---

### 📈 Future Improvements

- Use actual stock balances from live systems
- Add cost optimization and supplier constraints
- Scale to 100+ locations with performance tuning

---

### 🚀 Try It Yourself

If you'd like to test the system with your own data, just replace the input Excel file and run the notebook. The system will generate clean forecasts and reorder suggestions tailored to your data.

---

### 🔗 Connect With Me

If you found this project interesting, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/koushik-rangu-17a81328a/) or check out my other projects on [GitHub](https://github.com/Koushik050).

Let’s solve more real-world problems with data! 💡📊

```

---

