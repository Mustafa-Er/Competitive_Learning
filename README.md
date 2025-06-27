# 🧠 Competitive_Learning – Deep Learning K-Means Alternative

This project explores **Competitive Learning** as an unsupervised clustering algorithm, simulating its performance in recovering true cluster centers from synthetic data.  
Unlike traditional methods like **K-Means**, this approach draws inspiration from **biological neural networks**, where neurons "compete" to respond to input patterns.

---

## 🔁 Project Summary

- Investigates **Competitive Learning** as an alternative to K-Means for clustering tasks
- Demonstrates center convergence behavior under different learning rates
- Visualizes the training process dynamically for interpretability

---

## 🧪 Data Generation

Synthetic dataset created with a **two-stage process**:

1. **Center Initialization**  
   Randomly generate true cluster centers in an N-dimensional space.

2. **Sample Creation**  
   Generate noisy data points around each center to simulate real-world variance.

> 🎯 This setup allows direct comparison between **learned centers** and **ground-truth centers**.

---

## 🧠 Models & Training

Two **Competitive Learning** models were trained under different configurations (varying learning rates):

| **Model**     | **Learning Rate** | **Training Notes**                              |
|---------------|-------------------|--------------------------------------------------|
| Model 1       | `1e-2`            | Faster convergence; better approximation        |
| Model 2       | `1e-3`            | Slower updates; more gradual center adaptation  |

Both models used **winner-takes-all updates**, where only the "winning" unit (closest center) updated its weights toward the input sample.

![Training Curves](https://github.com/user-attachments/assets/2247246a-24f4-41f5-8851-5b8ad39186bd)

---

## 📉 Observations

- **Convergence Speed**:  
  Model 1 (higher learning rate) **converged faster** and aligned more closely with true centers.

- **Training Plateau**:  
  Both models plateaued after a certain number of epochs, indicating **training stabilization**.

- **Center Accuracy**:  
  Model 1 approximated the **true cluster centers** more accurately than Model 2.

---

## 🧩 Visualization

The learning process was visualized using animated plots to show **how the cluster centers moved** during training.

This made the **training dynamics** easy to understand and visually track:

![Center Movement Animation](https://github.com/user-attachments/assets/8e4d1e13-1fd1-478a-a718-a1b3c93daa1b)

---

## ✅ Conclusion

- **Competitive Learning** offers a compelling alternative to K-Means, particularly for biologically inspired or neural simulation environments.
- Learning rate plays a crucial role in **training speed** and **final accuracy**.
- Visualizing center dynamics over time helps reveal the **convergence behavior** of the algorithm.

