# 🚶‍♂️ Walking Trajectory Prediction: ML vs Signal Processing

This project presents a **comparative study** between **Machine Learning** models and **Signal Processing** techniques for **predicting walking trajectories** in real-time. We evaluated the performance using a **custom dataset** collected in a controlled environment.

---

## 🎯 Objective

To compare the **accuracy**, **robustness**, and **computational efficiency** of:

- 🧠 Machine Learning:
  - LSTM (Long Short-Term Memory)
  - GRU (Gated Recurrent Unit)

- 📈 Signal Processing:
  - Particle Filter (PF)
  - Kalman Filter (KF)

---

## 🧪 Dataset & Experimental Setup

- 📍 **Custom walking trajectory dataset**
- 🧍‍♂️ Data collected in a **controlled indoor environment**
- 📏 Evaluated at different trajectory completion stages: 70% and 90%

---

## 📊 Key Results

### ✅ At 70% of Trajectory:

| Model        | Accuracy (%) |
|--------------|--------------|
| **LSTM**     | **85.71**    |
| PF           | 64.61        |
| KF           | 43.07        |

- 🏆 LSTM outperformed both signal processing models in accuracy.
- 🔄 **PF showed superior robustness**, especially with **non-linear** paths:
  - 71.88% better in **Discrete Fréchet Distance (DFD)**
  - 25.71% better in **Root Mean Squared Error (RMSE)** compared to KF

---

### ✅ At 90% of Trajectory:

| Model        | Accuracy (%) |
|--------------|--------------|
| **LSTM**     | **90.48**    |
| PF           | 89.23        |
| GRU          | 80.95        |

- LSTM and PF performed **comparably well**.
- GRU showed decent performance but lagged slightly.

---

## 🔍 Insights

- 💡 **Machine Learning models** (LSTM, GRU) excel with **ample training data**, offering high accuracy.
- ⚙️ **Signal processing models** (PF, KF) are **more robust** in dynamic or data-scarce environments.
- ⚡ **PF** provides a **data-efficient, real-time** alternative when training data is limited.

---

## 🤖 Technology Stack

- 🐍 Python (NumPy, Pandas, Matplotlib)
- 📚 TensorFlow / PyTorch for LSTM & GRU
- 📐 Custom implementation of Particle and Kalman Filters
- 📊 Visualization and evaluation using DFD & RMSE

---

## 🌐 Applications

- 🏃 Human motion tracking
- 🤖 Mobile robot navigation
- 🧠 Smart environments
- 🧍 Elderly care and monitoring systems

---

## 🤝 Contributions

We welcome improvements, bug fixes, and new model experiments. Feel free to fork and open a pull request!

---

Understanding movement, predicting the future. 🚶‍♀️➡️🔮
