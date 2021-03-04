# Build:
# $ docker build --rm -f Dockerfile -t jshim/ros2_single_container .
#
# Run:
# $ docker run -it --rm jshim/ros2_single_container
#
# Pull:
# $ docker pull jshim/ros2_single_container

FROM osrf/ros:foxy-desktop
MAINTAINER jhshim@robotis.com

CMD ros2 run demo_nodes_cpp listener & ros2 run demo_nodes_cpp talker
