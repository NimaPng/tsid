# invdyn
C++ library for optimization-based inverse-dynamics control based on the rigid multi-body dynamics library [Pinocchio](https://github.com/stack-of-tasks/pinocchio).
Take a look at the project [wiki](https://github.com/stack-of-tasks/invdyn/wiki) for more details.

## Dependencies
* boost (unit_test_framework, serialization)
* eigen3
* [pinocchio](https://github.com/stack-of-tasks/pinocchio)

To install eigen3 on Ubuntu you can use apt-get:
  sudo apt-get install libeigen3-dev

To install [pinocchio](https://github.com/stack-of-tasks/pinocchio) follow the instruction on its website.

## Installation

    cd $DEVEL/openrobots/src/
    git clone --recursive git@github.com:stack-of-tasks/invdyn.git
    cd invdyn
    mkdir _build-RELEASE
    cd _build-RELEASE
    cmake .. -DCMAKE_BUILD_TYPE=RELEASE -DCMAKE_INSTALL_PREFIX=$DEVEL/openrobots
    make install