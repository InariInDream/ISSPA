# ISSPA (Intelligent Self-driving System Physical Agent)

This repo is used to develop and store codes for physical agents.

## Developing Environment

- Ubuntu 20.04

- ROS1 noetic

## WorkSpace Setup

Create a workspace for ROS:

```bash
mkdir ~/pa_ws/src -p
```

Clone the ISSPA codes:

```bash
cd ~/pavs/src
git clone https://github.com/chenhengwei1999/ISSPA.git
```

Install dependent libraries:

```bash
cd ~/pavs
rosdep install --from-paths src --ignore-src -r -y
```

Complie the whole projects using `catkin_make`:

```bash
catkin_make
```

Finally refresh the environment variables or store them in **.bashrc**.

```bash
source devel/setup.bash
```

## Usage Guide

### Quick Start of PVAS

When the **WorkSpace Setup** is completed, you can try the following tasks, which contain **vehicle chassis** startup, **sensor** startup, **remote control**, **SLAM**, and **navigation**. Refer [here](./docs/quick_start.md) for documentation.
