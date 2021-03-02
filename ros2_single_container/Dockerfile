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

CMD ros2 run demo_nodes_cpp listener & ros2 run demo_nodes_cpp talker
