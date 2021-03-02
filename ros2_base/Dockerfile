# Build:
# $ docker build --rm -f Dockerfile -t jshim/ros2_base .
#
# Run:
# $ docker run -it --rm jshim/ros2_base
#
# Pull: (Not supported yet)
# $ docker pull jshim/ros2_base

FROM osrf/ros:foxy-desktop
MAINTAINER jhshim@robotis.com

# install ros package
RUN apt-get update && apt-get install -y \
      ros-${ROS_DISTRO}-demo-nodes-cpp \
      ros-${ROS_DISTRO}-demo-nodes-py && \
    rm -rf /var/lib/apt/lists/*

# Not needed for the ros:foxy-desktop image
# COPY entrypoint.sh /entrypoint.sh
# RUN chmod +x /entrypoint.sh
# ENTRYPOINT ["/entrypoint.sh"]

# launch ros package
CMD ros2 launch demo_nodes_cpp talker_listener.launch.py
