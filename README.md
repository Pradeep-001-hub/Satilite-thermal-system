







## introduction:
This project focuses on the design and simulation of an optimal thermal control system for satellite applications using the Linear Quadratic Regulator (LQR). In space environments, thermal management is a critical subsystem due to the absence of convective heat transfer and the presence of highly variable radiative heat inputs such as solar radiation, Earth albedo, and eclipse conditions. These factors introduce significant thermal fluctuations that can degrade the performance and reliability of onboard electronic systems if not properly controlled.  

The aim of this work is to develop a control-oriented thermal model and apply optimal control techniques to maintain system temperatures within desired limits while minimizing energy consumption. The approach integrates principles from heat transfer and modern control theory to achieve a robust and efficient solution.


 LQR Controller Design  :
The control strategy is based on the Linear Quadratic Regulator, which computes an optimal state feedback gain matrix \( K \) that minimizes the quadratic cost function.

 algebraic Riccati equation:
A^T P + P A - P B R^{-1} B^T P + Q = 0

and computing:

K = R^{-1} B^T P

The resulting control law is:

u(t) = -Kx(t)

This approach ensures an optimal trade-off between temperature regulation accuracy and control effort, leading to improved system efficiency and stability.

## Simulation and Performance Analysis  
The system is implemented and simulated in MATLAB to evaluate its dynamic response. The LQR-controlled system demonstrates rapid convergence to the desired temperature with minimal overshoot and reduced settling time. Compared to conventional control strategies, the optimal controller provides smoother control action and better disturbance rejection. The results validate that the system remains stable under varying initial conditions and external thermal disturbances, confirming robustness.

Engineering Relevance  
Thermal control is a vital subsystem in satellite engineering, directly influencing mission reliability and component longevity. This project highlights the application of optimal control techniques in aerospace systems, aligning with real-world practices used in spacecraft thermal management. The integration of state-space modeling and LQR design reflects a strong foundation in modern control engineering, which is essential for advanced research and development.

## Future Enhancements  
The present work can be extended by incorporating nonlinear thermal effects and time-varying environmental conditions to improve model accuracy. The addition of a Kalman Filter for state estimation would enable handling of sensor noise and incomplete measurements, making the system more practical for real-world implementation. Further development may include hardware realization using embedded systems and real-time thermal sensors, bridging the gap between simulation and physical deployment.

