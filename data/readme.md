
# NASA Engine Degradation Dataset
## Overview
This dataset consists of multiple multivariate time series from a fleet of engines. Each engine operates normally at the start of the series and develops a fault that grows in magnitude until system failure. The objective is to predict the Remaining Useful Life (RUL) of each engine in the test set.

## Data Sets
### FD001
Train Trajectories: 100
Test Trajectories: 100
Conditions: ONE (Sea Level)
Fault Modes: ONE (HPC Degradation)
### FD002
Train Trajectories: 260
Test Trajectories: 259
Conditions: SIX
Fault Modes: ONE (HPC Degradation)
### FD003
Train Trajectories: 100
Test Trajectories: 100
Conditions: ONE (Sea Level)
Fault Modes: TWO (HPC Degradation, Fan Degradation)
### FD004
Train Trajectories: 248
Test Trajectories: 249
Conditions: SIX
Fault Modes: TWO (HPC Degradation, Fan Degradation)
## Experimental Scenario
The dataset includes multiple multivariate time series divided into training and test subsets. Each time series corresponds to a different engine, considered to be from a fleet of the same type. Engines start with different degrees of initial wear and manufacturing variation, which is normal and not considered a fault.

## Key Points:
Operational Settings: Three operational settings affect engine performance.
Sensor Noise: The data contains sensor noise.
Training Set: Fault grows until system failure.
Test Set: Time series ends before system failure.
Objective: Predict the number of remaining operational cycles before failure in the test set.
## Data Format
The data is provided as a zip-compressed text file with 26 columns of numbers, separated by spaces. Each row is a snapshot of data taken during a single operational cycle. The columns are:

- Unit number
- Time, in cycles
- Operational setting 1
- Operational" setting 2
- Operational setting 3
- Sensor measurement 1
- Sensor measurement 2
...
- Sensor measurement 26
## Reference
A. Saxena, K. Goebel, D. Simon, and N. Eklund, "Damage Propagation Modeling for Aircraft Engine Run-to-Failure Simulation", in the Proceedings of the 1st International Conference on Prognostics and Health Management (PHM08), Denver CO, Oct 2008.