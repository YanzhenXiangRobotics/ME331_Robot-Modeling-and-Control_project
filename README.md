# ME331-project

This is our final project of the course ME331: Modeling & Control of Robot at Southern University of Science and Technology(SUSTech). In this project, we mainly focus on trajectory tracking of the 3-DoF parallel delta robot. Basically, we use 5-order polynomial to conduct trajectory planning, and we apply four different control strategies to track the trajectory.
## Strategies & methods
![image](https://user-images.githubusercontent.com/54230111/127299693-7181d97d-a38f-4ffc-8d96-8577ead34155.png)
## Video demo
https://user-images.githubusercontent.com/54230111/127287669-a31f560d-4a44-4bb1-895d-7871cbc06db3.mp4
## Detailed descirptions
### Planned door-shaped trajectory
There are different caterories of curves that can be utilized to plan the door-shaped trajectory. Here we explores three kinds of curves: 5-oder polynomial curve, cycloidal curve and trajectory curve. And the comparison of the planned end-effector disposition v.s. time are illustrated as the follows.
![image](https://user-images.githubusercontent.com/54230111/127298846-8f67756c-3534-4907-8f99-e76de6c39010.png)
(horizontal)
![image](https://user-images.githubusercontent.com/54230111/127298859-04e4aa22-16de-443f-8adc-5b35a8b01f4f.png)
(vertical)
### Solidworks model
![image](https://user-images.githubusercontent.com/54230111/127298924-e5d1d5aa-4788-44d9-8fd6-93a704e46c0c.png)
### Simulink design & tracking results
#### Independent joint PID control without feedfoward
![image](https://user-images.githubusercontent.com/54230111/127299211-669c09a5-423a-4349-9f7e-6b670f0fdde1.png)
![image](https://user-images.githubusercontent.com/54230111/127299271-cf2e2643-9489-42c4-a898-5c7ceefa4e1a.png)
#### Independent joint PID control with feedfoward
![image](https://user-images.githubusercontent.com/54230111/127299297-bee33842-7922-4c8c-b3cc-50100f5b7761.png)
![image](https://user-images.githubusercontent.com/54230111/127299310-a4e369e8-2af8-4cf2-8d4c-3d8d80d3f2c0.png)
#### Computed torque control
![image](https://user-images.githubusercontent.com/54230111/127299336-56d0251f-e175-4816-a732-205d29e620b4.png)
![image](https://user-images.githubusercontent.com/54230111/127299349-8ec62c9c-6042-40d3-b604-aa90400743b9.png)
#### Nonlinear feedback control
![image](https://user-images.githubusercontent.com/54230111/127299397-bc8bce34-ddd1-47b7-b0d7-b47fa64fae88.png)
![image](https://user-images.githubusercontent.com/54230111/127299409-e49f00d7-4530-4a53-a122-a6be9271d519.png)
## Folder & file structures
Traj_planning: codes related to trajectory planning
IK_ID: codes related to IK & ID calculations
Tracking_simulation: codes, ADAMS plants & SIMULINK models related to tracking simulation using 1) PID without feedfoward (SIMULINK: delta_pid.slx); 2) PID with feedfoward (SIMULINK: delta_pid_FFW.slx); 3) Computed torque control (SIMULINK: delta_CTC.slx) 4) Nonlinear feedback control (SIMULINK: delta_nonlinear.slx). 
## Team members
Yanzhen Xiang; Nuo Chen; Xiaoyu Yan; Shangkun Guo; Zhiyuan Han
