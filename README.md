# ME331-project

This is our final project of the course ME331: Robot Modeling & Control at Southern University of Science and Technology(SUSTech). 3-DoF delta robot is a kind of robot that is pervalently used in garbage sorting automation, and it is crucial for the robot to traverse a certain trajectory to reach the target. In this project, we mainly focus on trajectory planning and tracking of the 3-DoF parallel delta robot. 5-order polynomial is used to plan trajectory, and four different control strategies are applied to track the trajectory: independent PID control without feedforward, independent PID control with feedforward, computed torque control and nonlinear feedback control. Under the four strategies, the trakced trajetories are all quite close to the planned trajectory, serving as validations for the strategies.
## Video demo
https://user-images.githubusercontent.com/54230111/127287669-a31f560d-4a44-4bb1-895d-7871cbc06db3.mp4
## Strategies & methods
<img src=https://user-images.githubusercontent.com/54230111/127299693-7181d97d-a38f-4ffc-8d96-8577ead34155.png width=500 height=400 />

## Detailed descirptions

### Planned door-shaped trajectory
There are different caterories of curves that can be utilized to plan the door-shaped trajectory. Here we explores three kinds of curves: 5-oder polynomial curve, cycloidal curve and trajectory curve. And the comparison of the planned end-effector disposition v.s. time are illustrated as the follows.
<center>
<figure>
<img src=https://user-images.githubusercontent.com/54230111/127301705-0778b9fd-1927-4373-8369-b64ad62ddcd3.png width=400/>
<img src=https://user-images.githubusercontent.com/54230111/127301764-295857a7-15f8-4546-90c1-d0b7fdcbb745.png width=400/>
</figure>
  
### Solidworks model
  
<img src=https://user-images.githubusercontent.com/54230111/127302956-f701b768-1763-4e38-b347-72591fcc906f.png width=500 height=400 />
  
### Simulink design & tracking results
  
#### Independent joint PID control without feedfoward
  
<img src=https://user-images.githubusercontent.com/54230111/127299211-669c09a5-423a-4349-9f7e-6b670f0fdde1.png width=800 height=500 />
<img src=https://user-images.githubusercontent.com/54230111/127299271-cf2e2643-9489-42c4-a898-5c7ceefa4e1a.png width=500 height=400 />

#### Independent joint PID control with feedfoward
  
<img src=https://user-images.githubusercontent.com/54230111/127299297-bee33842-7922-4c8c-b3cc-50100f5b7761.png width=800 height=500 />
<img src=https://user-images.githubusercontent.com/54230111/127299310-a4e369e8-2af8-4cf2-8d4c-3d8d80d3f2c0.png width=500 height=400 />

#### Computed torque control
 
<img src=https://user-images.githubusercontent.com/54230111/127299336-56d0251f-e175-4816-a732-205d29e620b4.png width=800 height=500 />
<img src=https://user-images.githubusercontent.com/54230111/127299349-8ec62c9c-6042-40d3-b604-aa90400743b9.png width=500 height=400 />
  
#### Nonlinear feedback control
  
<img src=https://user-images.githubusercontent.com/54230111/127299397-bc8bce34-ddd1-47b7-b0d7-b47fa64fae88.png width=800 height=500 />
<img src=https://user-images.githubusercontent.com/54230111/127299409-e49f00d7-4530-4a53-a122-a6be9271d519.png width=500 height=400 />
  
  
## Folder & file structures
  
Traj_planning: codes related to trajectory planning
IK_ID: codes related to IK & ID calculations
Tracking_simulation: codes, ADAMS plants & SIMULINK models related to tracking simulation using 1) PID without feedfoward (SIMULINK: delta_pid.slx); 2) PID with feedfoward (SIMULINK: delta_pid_FFW.slx); 3) Computed torque control (SIMULINK: delta_CTC.slx) 4) Nonlinear feedback control (SIMULINK: delta_nonlinear.slx). 
  
## Team members
Yanzhen Xiang; Nuo Chen; Xiaoyu Yan; Shangkun Guo; Zhiyuan Han
