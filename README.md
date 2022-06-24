# Cruise controller for car
## This project aims towards driving car's velocity to specific value.


<img src="https://user-images.githubusercontent.com/92177410/160154176-ba6324f2-1548-4d1d-975f-b0ba487fb28b.png" width="400" height="200">

#### PID CONTROLLER

  
<img src="https://user-images.githubusercontent.com/92177410/160156713-d0ec7dbc-0caa-4295-a781-0e32baa81d9b.png" width="400" height="150">


- For a given referce value , error is calculated by subracting refernce value and current value.
- This error is feed to PID controller , where corresponding proportional, derivative and intergral gains are computed to get desired force to drive car.
- As time approach infinity, velocity approach desired value.
### Physics:

 v = u + a(t2 - t1)
- v and u are final and initial velocity respectively.
- a is acceleration 
- (t2 - t1) is time step which we have taken as 1 second.
 
 
 F = ma
 
 - F is input to system over which we apply our control law.
 ### Results:
 
  
 ### single desired velocity:

 Desired velocity -> 60 km\hr


**Only Proportional gain Kp:**

 - Only Kp value does not make car's velocity reach its desired velocity
 
 
**Proportional and Integral gain:**
 
 - Integral gain add up errors making velocity reach desired velocity but overshoots abit.
 
  
  **Proportional, Integral and Derivate gain:**
  
 - Derivate gain reduces the overshoot and for some value velocity smoothy converges to desired velocity 
  
 
![image](https://user-images.githubusercontent.com/86155751/175607482-3191fd2e-f0f4-4807-a8f0-64d20a563e26.png)







