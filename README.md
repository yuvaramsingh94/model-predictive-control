# model-predictive-control

#### The MPC model

the model is inspired from Udacity's MPC course . here i have used car's x,y,velocity, psi,cte, error of psi as teh state vectors and two controls speed , steering angle . the model predicts the best set of control input which has low cost by trying out a combination of input controls . 

#### Timestep Length and Elapsed Duration (N & dt)

after trying many combination of values and going through the walkdown video provided by udacity , i choose N = 10 and dt = 0.1 . 

#### Polynomial Fitting and MPC Preprocessing

as suggested in the walkthrough video , i just converted the wy points to car centric points and fit a polynomial onto it . 

#### Model Predictive Control with Latency

after going through various notes , previous student works i just add delay to the actuation commands and found it to be working with the latency . i did get inspired from other students work 
