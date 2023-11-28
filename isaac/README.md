\[Reference\]:
  * https://github.com/NVIDIA-ISAAC-ROS/isaac_ros_nvblox
  * https://developer.nvidia.com/blog/design-your-robot-on-hardware-in-the-loop-with-nvidia-jetson/

\[Quickstart\]:

\[1\]. Set up your development environment by following the instructions here (https://github.com/NVIDIA-ISAAC-ROS/isaac_ros_common/blob/main/docs/dev-env-setup.md) .

\[2\]. Clone this repository and its dependencies under /ssd/workspaces/isaac_ros-dev/src.

```
$ cd /ssd/workspaces/isaac_ros-dev/src
$ git clone https://github.com/NVIDIA-ISAAC-ROS/isaac_ros_common
$ git clone --recurse-submodules https://github.com/NVIDIA-ISAAC-ROS/isaac_ros_nvblox && \
    cd isaac_ros_nvblox && git lfs pull
```

\[3\]. Pull down a ROS Bag of sample data:

```
$ cd /ssd/workspaces/isaac_ros-dev/src/isaac_ros_nvblox && \
  git lfs pull -X "" -I "nvblox_ros/test/test_cases/rosbags/nvblox_pol"
```

\[4\]. Launch the Docker container using the run_dev.sh script:

```
$ cd /ssd/workspaces/isaac_ros-dev/src/isaac_ros_common && \
  ./scripts/run_dev.sh ${ISAAC_ROS_WS}
```

\[5\]. Inside the container, install package-specific dependencies via rosdep:

```
$ cd /workspaces/isaac_ros-dev/ && \
    rosdep install -i -r --from-paths src --rosdistro humble -y --skip-keys "libopencv-dev libopencv-contrib-dev libopencv-imgproc-dev python-opencv python3-opencv nvblox"
```

\[6\]. Build and source the workspace:

```
$ cd /workspaces/isaac_ros-dev && \
  colcon build --symlink-install && \
  source install/setup.bash
```

\[7\]. (Optional) Run tests to verify complete and correct installation:

```
$ colcon test --executor sequential
```

\[8\]. In a current terminal inside the Docker container, run the launch file for Nvblox with nav2:

```
$ source /workspaces/isaac_ros-dev/install/setup.bash && \
    ros2 launch nvblox_examples_bringup isaac_sim_example.launch.py
```

\[9\]. Open a second terminal inside the docker container:

```
$ cd /ssd/workspaces/isaac_ros-dev/src/isaac_ros_common && \
  ./scripts/run_dev.sh ${ISAAC_ROS_WS}
```

\[10\]. In the second terminal, play the ROS Bag:

```
$ ros2 bag play src/isaac_ros_nvblox/nvblox_ros/test/test_cases/rosbags/nvblox_pol
```

You should see the robot reconstructing a mesh, with the 2d esdf slice overlaid on top.
