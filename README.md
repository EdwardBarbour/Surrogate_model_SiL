## Developing a surrogate model based on OpenFAST data for Software in the Loop (SiL)

This code accompanies a paper in development 'Scaled physical modelling of floating offshore wind turbines using a neural network surrogate  model for aerodynamic emulation' by Edwards _et. al._

All code is contained within the jupyter notebook and uses the demo file output from OpenFAST.

The OpenFAST file is for the VolturnUS-S, a three-column semi-submersible platform with the 15 MW IEA turbine. <br>
The system is run for an average windspeed of $11ms^{-1}$, a Turbulence Intensity of 15%,a  significant wave height of 1.8m and waver period 16.5s. The ROSCO controller is turned ON. <br>

Firstly, features are engineered based on the OpenFAST demo file and then a Multiple Linear Regression (MLR) model is used to predict the thrust on the tower and turbine. <br>
Secondly an Artifical Neural Network (ANN) is developed with the same input features and used for thrust prediction. <br>
Finally, the errors of both approaches are compared. Code is also included to show how the weights and biases are extracted from the ANN and used.

In the lab, this is done in MATLAB as described in Edwards _et. al._

