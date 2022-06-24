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

**only proportional gain Kp:**
 only Kp value does not make car's velocity reach its desired velocity
 
 
 <img width="295" alt="ki=0   kd=0" src="https://user-images.githubusercontent.com/92177410/160253422-814f4004-a0b0-4431-939f-95e1f2a951a3.png">
 
 
 
**proportional and integral gain:**
 
 Integral gain add up errors making velocity reach desired velocity but overshoots abit.
 
<img width="311" alt="kd=0" src="https://user-images.githubusercontent.com/92177410/160253519-963acd29-1cfa-4e9c-90d4-d1da9b0b4990.png">
  
  
  **proportional, integral and derivate gain:**
  
  Derivate gain reduces the overshoot and for some value velocity smoothy converges to desired velocity 
  
 
 
<img width="282" alt="Screenshot 2022-03-21 230711" src="https://user-images.githubusercontent.com/92177410/160253626-da6ce142-e8f5-472d-9a19-c6f5bf153e5c.png">





<img width="294" alt="variable desired velocity" src="https://user-images.githubusercontent.com/92177410/160253895-8adc3123-6ccb-4e43-8e81-1e7eaadef8ca.png">

