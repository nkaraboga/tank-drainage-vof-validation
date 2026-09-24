3D transient CFD simulation and analytical validation of gravity-driven tank drainage using ANSYS Fluent (VOF) .

This study was inspired by and built upon the tank emptying workshop material presented by Sijal Ahmed. Special thanks to him for sharing his CFD methodologies and reference case setup.

In this study, the gravity-driven drainage of a cylindrical water tank through a bottom orifice was simulated using ANSYS Fluent (3D) and CFD-Post. The numerical results were validated against the analytical discharge equation (Torricelli's Law).

Geometry and Analytical Calculation
 Tank Diameter (D): 0.01414 m (Area A = 1.57e-4 m²)
 Tank Height (H): 0.0257 m
 Orifice Diameter (d): 0.002 m (Area a = 3.14e-6 m²)
 Discharge Coefficient (Cd): 0.81

Theoretical emptying time is calculated as:
  t = (2 * A) / (Cd * a * sqrt(2 * g)) * sqrt(H)
  Analytical Emptying Time = 4.45 s


Mesh Parameters
 Mesh Type: 3D Hexahedral - Sweep Mesh
 Elements: 54432
 Nodes: 56815
 Average Orthogonal Quality: 0.88
 Average Skewness: 0.21


 Solver and Simulation Setup
   Solver: 3D, Pressure-Based, Transient
   Multiphase Model: Volume of Fluid (VOF) (Air as primary, Water as secondary)
   Turbulence Model: Realizable k-epsilon
   Time Stepping: Adaptive time stepping (CFL guided)


 Results Comparison
   Analytical Time: 4.45 s
   ANSYS Fluent Time: 4.42 s
   Relative Error: 0.67%


