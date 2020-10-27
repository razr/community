# Test environment

This document defines the test environment for the ROS2 real-time tests

The goal is to provide a reproducible test environment.

## Hardware

For the tests we plan to use an affordable hardware based on x86_64 and ARM v8 architectures. It shall be easy to acquire, to use it and it shall provide a good software support. Here is a requirements list:
* Harwdare architecture
    * Intel x86_64
    * ARM v8
* min 4 cores
* min 8 GB RAM
* supports Ubuntu 20.04

### ARM

* [Raspberry Pi4 8 GB RAM, 4 cores](https://www.raspberrypi.org/blog/8gb-raspberry-pi-4-on-sale-now-at-75)

### Intel

* [UP squared 8 GB RAM, 4 cores](https://up-shop.org/up-squared-board-pentium-quad-core-8gb-memory-64gb-emmc.html)

## Software

For the tests we plan to use software the ROS2 is built and tested upon. Here is a requirements list

* Ubuntu 20.04 LTS (iso image)
    * [Raspberry Pi4](https://ubuntu.com/download/raspberry-pi)
    * [UP squared]( https://wiki.up-community.org/Ubuntu)
* PREEMPT_RT Kernel, maybe a newer than one provided by Ubuntu 20.04, depending on the available features

### Kernel

* [PREEMPT_RT Kernel](https://wiki.linuxfoundation.org/realtime/start) is built based on the specific RT Test configuration 
* a docker based kernel build
