---
key: "radar_param_est"

order: 4

name: "Estimating adaptive cruise control model parameters from on-board radar units"

description: "<p> This project explores methods for model parameter estimation on a car-following model using data collected from Adaptive Cruise Control (ACC) enabled vehicles. The proposed methods are batch method least-squares and an online particle filter. Numerical experiments demonstrate the accuracy and computational performance of the methods relative to a commonly used simulation-based optimization approach. The methods are also assessed on empirical data collected from a 2019 model year ACC vehicle driven in a highway environment. Speed, space gap, and relative velocity data are recorded directly from the factory-installed radar unit via the vehicle’s CAN bus. The least-squares method has the fastest run-time performance, and is up to 3 orders of magnitude faster than other methods. The particle filter is faster than real-time, and therefore is suitable in streaming applications in which the datasets can grow arbitrarily large."

funding: "National Science Foundation"

students: "Yanbing Wang, George Gunter"

image: /images/radar_all_track.png
---
