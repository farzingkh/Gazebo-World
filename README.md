[![Udacity - Robotics NanoDegree Program](https://s3-us-west-1.amazonaws.com/udacity-robotics/Extra+Images/RoboND_flag.png)](https://www.udacity.com/robotics)

# RoboND-myWorld
The **myrobot** lab part of RoboND Gazebo Basics lesson. The purpose of this lab is to learn how to build a two-wheeled robot model with the Model Editor tool in Gazebo. Include this model in an empty Gazebo World. And, finally write a plugin to interact with this world.  

### Directory Structure
<pre><font color="#3465A4"><b>.</b></font>
├── CMakeLists.txt
├── <font color="#3465A4"><b>images</b></font>
│   └── <font color="#75507B"><b>output.png</b></font>
├── <font color="#3465A4"><b>model</b></font>
│   ├── <font color="#3465A4"><b>armOnCart</b></font>
│   │   ├── model.config
│   │   └── model.sdf
│   ├── <font color="#3465A4"><b>cartArm</b></font>
│   │   ├── model.config
│   │   └── model.sdf
│   └── <font color="#3465A4"><b>myBuilding</b></font>
│       ├── model.config
│       └── model.sdf
├── README.md
├── <font color="#3465A4"><b>script</b></font>
│   └── hello.cpp
└── <font color="#3465A4"><b>world</b></font>
    └── myOffice
</pre>                   
```

### Steps to launch the simulation

#### Step 1 Update and upgrade the Workspace image
```sh
$ sudo apt-get update
$ sudo apt-get upgrade -y
```

#### Step 2 Clone the lab folder in /home/workspace/
```sh
$ cd /home/workspace/
$ git clone https://github.com/udacity/RoboND-myrobot myrobot
```

#### Step 3 Compile the code
```sh
$ cd /home/workspace/myrobot/
$ mkdir build
$ cd build/
$ cmake ../
$ make
```

#### Step 4 Add the library path to the Gazebo plugin path  
```sh
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/myrobot/build
```

#### Step 5 Run the Gazebo World file  
```sh
$ cd /home/workspace/myrobot/world/
$ gazebo myworld
```

### Output
The hello world message and the two-wheeled robot inside a Gazebo World should both launch as follow: 
![alt text](images/output.gif)


    
 
