# **Link to TurtleBot Team 2 Videos** :
[Download Videos](https://we.tl/t-w6U39jeaVv)

## **USAGE - follow_me** :

1. Unzip the `follow_me.zip` package.
2. Place the entire `follow_me` folder in `~/turtlebot3_ws/src/`.
3. Run the command: `colcon build`
4. Source the bash environment.
5. Run the command: `ros2 run follow_me follow_me_node`

## **USAGE - burger.yaml** :

1. Place the file in `~/turtlebot3_ws/src/turtlebot3/turtlebot3_navigation2/param/`.
2. Replace the existing file.

This setup file will be used by the TurtleBot's Nav2 package. It includes the MPPI Controller setup.

## **USAGE - BH_follow_me.xml** :

1. Refer to the following tutorial:
   [Navigation2 Dynamic Point Following](https://docs.nav2.org/tutorials/docs/navigation2_dynamic_point_following.html).
   - Follow the instructions under "1- Setup Rviz clicked point".
   - Follow the instructions under "2- Run Dynamic Object Following in Nav2 Simulation".



# Challenge TurtleBot3
## Phase 1
- **Result:** Failure  
- **Comment:** 
  - `Follow_me` script does not follow entirely. 
  - Inversed direction in reverse when a person is too close to the robot.
---
## Phase 2
- **Result:** Mitigated  
- **Static Obstacle:** Yes  
- **Dynamic Obstacle:** Yes  
- **Blocked Path:** Yes  
- **Comment:** 
  - `Goto` works perfectly but is only usable with Rviz IHM. 
  - `Goto_pose` topic command is not working.
---
## Phase 3
- **Result:** Failure  
- **Comment:** 
  - Same as Phase 2, not yet implemented in the launch file.

