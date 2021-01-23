# CSE 3901 Basic Environment

This repo contains the basic environment for the CSE 3901 Web Apps class in a docker container designed to be used with the VSCode `Remote - Containers` extension. It comes with ruby and rails preinstalled and a VNC server for any applications that require a local GUI.

## Installation

1. Download Docker
2. Install VSCode and the `Remote - Containers` extension for VSCode
3. Run `Remote - Containers: Rebuild and Reopen in Container` in VSCode
4. Connect to port 5900 with a VNC client to access VNC server

## Adding gems or apt packages

If gems or apt packages are needed for a project you can add them to the Dockerfile in the `.devcontainer` folder. Add them near the end so that the entire container isn't rebuilt.

## Configuring VNC Server

The VNC server is run with the `/startup.sh` script. Documentation on configuring this script can be found in [the ubuntu-desktop-lxde-vnc image on docker hub](https://hub.docker.com/r/dorowu/ubuntu-desktop-lxde-vnc/)
