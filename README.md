# Udacity Student Project: Solve Localization Problem using AMCL
A Udacity student project to solve localization problem using ROS AMCL &amp; Navigation Stack.

In this project, students will learn the following:

- Accurately localizing a mobile robot inside a provided map in the Gazebo and RViz simulation environments.

- Building a mobile robot for simulated tasks.

- Creating a ROS package that launches a custom robot model in a Gazebo world and utilizes packages like AMCL and the Navigation Stack.

- Exploring, adding, and tuning specific parameters corresponding to each package to achieve the best possible localization results.

Full report can refer to [here](localization_where_am_i.pdf).

## Installation Instructions

The project can be completed in the provided Udacity Workspace in the Classroom. Alternatively, it can be completed on an Ubuntu System with ROS Kinetic installed on it. Some specific ROS packages might be required in order to complete the project -

``` bash
$ sudo apt-get install ros-kinetic-navigation
$ sudo apt-get install ros-kinetic-map-server
$ sudo apt-get install ros-kinetic-move-base
$ rospack profile
$ sudo apt-get install ros-kinetic-amcl
```

Once all the packages are installed, clone the repository on your system and rename the project folder to `udacity_bot`. However, it is recommended that you follow the Classroom instructions on working through the project instead of cloning the repo.


## Run the Project

After completing the project, you can launch it by running the following commands first -

```bash
$ cd ~/catkin_ws
$ catkin_make
$ source devel/setup.bash
```

And then run the following in *separate* terminals -

``` bash
$ roslaunch udacity_bot udacity_world.launch
$ roslaunch udacity_bot amcl.launch
$ rosrun udacity_bot navigation_goal
```
