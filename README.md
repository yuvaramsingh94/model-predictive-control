

# model-predictive-control

#### The MPC model

the model is inspired from Udacity's MPC course . here i have used car's x,y,velocity, psi,cte, error of psi as teh state vectors and two controls speed , steering angle . the model predicts the best set of control input which has low cost by trying out a combination of input controls . 

this is the model which i used in this MPc to control the car . it has x,y,orientation , velocity , cross track error and psi error

![state](./state.png)

#### Timestep Length and Elapsed Duration (N & dt)

after trying many combination of values and going through the walkdown video provided by udacity , i choose N = 10 and dt = 0.1 . 

#### Polynomial Fitting and MPC Preprocessing

as suggested in the walkthrough video , i just converted the wy points to car centric points and fit a polynomial onto it . 

#### Model Predictive Control with Latency

after going through various notes , previous student works , i found out that the actuation is based on the previous state . the latency of 100 milliseconds makes this actuation of no use because the current state is different from the measured state . 
