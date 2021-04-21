# 419_Quad_Stabilization: Automatic Quadcopter Launching Under Unstructured Conditions

This branch is called "dev_from_202004", which means it is a new start from April 2020. 

(1) Compile ROS package CrazyS
(2) Customize launch files in ./launchs, or world files in ./worlds

---

Flexible launching of a quadrotor system remains challenging due to its highly dynamical nature. Generally, the popular commercial quadrotor (e.g., [DJI](https://www.dji.com/)) requires a trained operator to execute the launching on a plain ground with remote control. Such requirements cannot be always satisfied under certain extreme environments or emergencies. In this project, the objective is to design an automatic launching module using reinforcement learning (RL) for a nano-quadrotor system ([Crazyflie 2.1](https://www.bitcraze.io/products/crazyflie-2-1/)), which supports more flexible launching under unstructured conditions, such as rugged ground and hand-throwing. As a short-term goal, one can first teach a quadrotor how to launch from a plain ground.

The [Gazebo simulator](http://gazebosim.org/) can provide accurate physical modelling of quadrotor and allow for efficient and safe training for this task. One can use neural network as a powerful, non-linear controller and select the state-of-art RL algorithm, either model-free or model-based one, to optimize the controller to achieve stable launching in simulation. Then the controller needs to be transferred and fully fine-tuned from simulation to real system. Finally, put this special quadrotor on the ground and witness the magic of neuro-based fully automatic launching! 
