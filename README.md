# Competitive_Learning
Deep Learning K-Means

🔁 Competitive Learning for Clustering Simulation
This project explores Competitive Learning as an alternative to K-Means for clustering tasks, particularly focusing on how well it can recover the true centers of synthetic data.

📌 Project Summary
Unlike traditional clustering approaches like K-Means, this project investigates Competitive Learning – a biologically inspired unsupervised learning technique – to cluster data points based on similarity.

🧪 Data Generation
The dataset is fully synthetic and generated in two stages:

Center Initialization: Randomly generate a few cluster centers in N-dimensional space.

Sample Creation: Around each center, generate random data points by adding small random variations (noise).

This controlled setup allows for a ground-truth comparison of the learned centers versus the true ones.

🧠 Models & Training
Two competitive learning models were trained with different configurations:

![image](https://github.com/user-attachments/assets/2247246a-24f4-41f5-8851-5b8ad39186bd)


Both models used competitive weight updates, where only the "winning" neuron updates its weights toward the input sample.

📉 Observations
Convergence Speed: The model with a higher learning rate (1e-2) converged faster to reasonable center positions. This aligns with expectations.

Training Plateau: Both models showed diminishing returns after a certain number of epochs, indicating stabilization.

Center Comparison: At the end of training, both models’ learned centers were compared with the true centers.

✅ Model 1 (higher learning rate) approximated the true centers more accurately than Model 2.

🧩 Visualization
The learning process of both models was visualized using animations that showed how the centers moved during training. This made it easier to interpret the convergence behavior dynamically.

![image](https://github.com/user-attachments/assets/8e4d1e13-1fd1-478a-a718-a1b3c93daa1b)


