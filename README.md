✈️ Global Aviation Network Resilience & Pandemic Dynamics

🎓 Social Networks Course Project — An empirical network science and data visualization pipeline built as the final project for the Social Networks course. This project models the global aviation infrastructure (3,188 airports, 36,860 routes) to analyze structural vulnerabilities, detect geopolitical communities, and simulate pandemic spreading dynamics under adaptive global lock-down policies.

📌 Project Overview

This project treats the global aviation network as a complex directed graph. By integrating graph theory, percolation physics, and epidemiological modeling, the pipeline provides actionable insights into how structural design dictates both economic robustness and global pandemic vulnerability.

The theoretical foundation of this analysis is calibrated against the classic network science models described in Albert-László Barabási's Network Science literature.

🎨 Preview & Visual Showcase

🗺️ Global Flight Trajectories (Geospatial Mapping)

Nodes represent airports scaled by out-degree centrality; edges trace active directed routes mapped to actual coordinates.

🦠 Spreading Dynamics Comparison

Comparing a standard unhindered viral outbreak against an adaptive policy intervention that effectively flattens the curve.

Standard SIR Model (No Intervention)

Adaptive SIR Model (Flattening the Curve)





🎨 Louvain Geopolitical Partitioning & Scale-Free Proof

How density dictates geography (automatic grouping into continental communities) along with the log-log degree distribution.

Community Detection (Louvain)

Log-Log Degree Distribution





🛡️ Targeted Attack Resiliency (Percolation Curves)

Comparing system resilience under random node deletion (green) vs. targeted hub removal (red).

🎬 Live Contagion Propagation (Spreading Animation)

A dynamic geospatial simulation showcasing real-time viral propagation across global flight corridors.

🚀 Key Features

🔍 1. Topological Profiling

Small-World Dynamics: Proves the "six degrees of separation" in physical transit, showing a short Network Diameter ($\text{Diameter} = 12$) paired with high local clustering ($\approx 0.49$).

Scale-Free Architecture: Leverages log-log cumulative degree distribution plots to mathematically prove the power-law degree distribution characteristic of preferential attachment networks.

Gatekeeper Discovery: Employs Betweenness Centrality to identify hidden logistical bottlenecks (such as Anchorage Airport, Alaska) acting as vital bridges across disconnected geographical communities.

🛡️ 2. Percolation & Robustness Simulations

Random Failures: Simulates system recovery under random node failures (weather-induced local delays).

Targeted Attack Resiliency: Models systematic network collapse under coordinated attacks targeting high-degree hubs, revealing a critical percolation threshold ($f_c \approx 10-15\%$).

🎨 3. Geospatial Community Detection

Unsupervised Partitioning: Runs the Louvain Modularity algorithm to group airports into 20 highly distinct geographical communities ($Q = 0.6548$).

Spatial Homophily: Demonstrates how flight densities naturally mirror geographical continents and political boundaries without feeding coordinates to the clustering algorithm.

🦠 4. Adaptive Spreading Dynamics

The Zero-Threshold Dilemma: Illustrates why pandemics spread instantly in Scale-Free networks due to an epidemic threshold approaching zero ($\lambda_c \to 0$).

Policy Interventions & Curve Flattening: Demonstrates the mathematical efficacy of timely flight bans (dropping transmission $\beta$ from $12\%$ to $2\%$).

🛠️ Installation & Tech Stack

This project is built entirely in Python using standard scientific computing and graph libraries:

# Clone the repository
git clone [https://github.com/yourusername/global-aviation-network-resilience.git](https://github.com/yourusername/global-aviation-network-resilience.git)

# Install dependencies
pip install networkx pandas matplotlib numpy python-louvain pillow

# Launch the analysis pipeline
jupyter notebook aviation_analysis.ipynb


📂 Repository Structure

├── README.md               # Interactive portfolio showcase
├── aviation_analysis.ipynb # Fully-documented Jupyter Notebook pipeline
├── data/                   # Cleaned OpenFlights datasets
│   ├── airports.dat
│   └── routes.dat
└── visualizations/         # Generated high-resolution plots & animations
    ├── adaptive_sir_simulation.png
    ├── community_detection.png
    ├── degree_distribution.png
    ├── geospatial_network.png
    ├── live_epidemic_spread.gif
    ├── robustness_curves.png
    └── sir_simulation.png


🎓 References

Barabási, A.-L. (2016). Network Science. Cambridge University Press. Online version at networksciencebook.com.

OpenFlights Airport and Route Database: openflights.org/data.

Developed with ❤️ by Mahmoud Abdel Nasser