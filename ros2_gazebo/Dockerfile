# Build:
# $ docker build --rm -f Dockerfile -t jshim/ros2_gazebo .
#
# Run:
# $ rocker --x11 --nvidia --name ros2_gazebo jshim/ros2_gazebo
#
# Pull:
# $ docker pull jshim/ros2_gazebo

FROM osrf/ros:foxy-desktop
MAINTAINER jhshim@robotis.com

RUN apt-get update \
  && apt-get install -q -y --no-install-recommends ros-foxy-gazebo-dev

CMD gazebo
