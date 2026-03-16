

# 📊 1. Linear Regression Forecast (1/1/25)

Using:

y = a + bt

### Calculated values:

* Slope ( b = -0.4283 )
* Intercept ( a = 63.0045 )

### Forecast:

[
\hat{y} = 63.0045 + (-0.4283 \times t)
]

For next period (1/1/25):

**Forecast = 10.75**

---

# 📈 2. Moving Average (4 Periods)

MA_4 = \frac{y_t + y_{t-1} + y_{t-2} + y_{t-3}}{4}

Using last 4 values:

**MA(4) Forecast = 15.99**

---

# 📉 3. Moving Average (12 Periods)

MA_{12} = \frac{y_t + y_{t-1} + \cdots + y_{t-11}}{12}

Using last 12 values:

**MA(12) Forecast = 15.61**

---

# 📊 4. Which Forecast is More Accurate?



**Moving Average (12) is likely more accurate**

### Why:

* Your regression slope is **negative (-0.428)** → shows downward trend
* But regression forecast (**10.75**) is **much lower** than recent values (~15–16)
* This suggests regression is **overfitting long-term decline**

MA(12) is better because:

* It smooths fluctuations
* Reflects **recent stable price level**
* Less affected by extreme past values

---

# 5. In-Depth Explanation

### 🔹 Linear Regression Result

* Indicates a **downward trend in prices**
* Predicts a sharp drop to **10.75**
* Meaning:
  👉 “Model assumes decline will continue strongly”

⚠️ Limitation:

* Uses entire dataset → influenced by older values
* Not ideal if recent prices stabilized

---

### 🔹 MA(4) Result (15.99)

* Focuses on **last 4 periods**
* Very responsive to recent changes

👉 Meaning:
“Short-term market behavior”

⚠️ Limitation:

* Can fluctuate a lot (less stable)

---

### 🔹 MA(12) Result (15.61)

* Uses more data → smoother
* Reflects **true current level**

👉 Meaning:
“Stable estimate of current price”

---

# 🎯 Final Conclusion

“The linear regression model predicts a lower closing price due to a downward trend in the overall dataset. However, the moving average forecasts are higher because they rely more on recent data. The 12-period moving average is likely the most accurate as it provides a balanced and stable estimate by smoothing short-term fluctuations while still reflecting current price behavior.”


* I can generate **Google Colab Python code**
* Or create a **graph comparing all 3 forecasts (professors love this)**
