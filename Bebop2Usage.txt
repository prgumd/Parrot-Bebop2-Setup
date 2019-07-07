Bebop2Usage.txt

1. Connect to Bebop 2 Wifi
2. 
```roscore```
3. ```roslaunch bebop_driver bebop_node.launch```
4. Use the following commands to do specific tasks:
Takeoff:
```rostopic pub --once /bebop/takeoff std_msgs/Empty```
Land:
```rostopic pub --once /bebop/land std_msgs/Empty```
Movement:
```rostopic pub --once /bebop/cmd_vel geometry_msgs/Twist "linear:
  x: 0.0
  y: 0.0
  z: 0.0
angular:
  x: 0.0
  y: 0.0
  z: 0.0" ```

Change values of x,y,z as needed.
5. To enable camera without stabilization
    ```~/bebop_ws/./video_stabil.sh```
