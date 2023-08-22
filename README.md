# Video Call Application

This script implements a simple video call application using OpenCV and Tkinter. It provides the ability to either send live video from your webcam to a specified directory on a web server or receive and display video from a specified IP address.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Functionality](#functionality)
    - [Send Video](#send-video)
    - [Receive Video](#receive-video)
- [Requirements](#requirements)
    - [Running Environment](#running-environment)
    - [Firewall and SELinux](#firewall-and-selinux)

## Prerequisites

- Python 3.x
- OpenCV (`cv2` library)
- Tkinter (usually included with Python)
- `wget` command-line tool

## Usage

1. Install the required packages using `pip install opencv-python-headless`.
2. Install the required packages using `pip install yum install python3-tkinter`.
3. Copy the provided code into your Python script or file.
4. Run the script using `python finalcode.py`.

## Functionality

### Send Video

The script captures video from the webcam and continuously saves frames as images in the specified directory on the web server. Press the Enter key to stop sending video.

### Receive Video

The script downloads images from the specified IP address and displays them as a video stream. Press the Enter key to stop receiving video.

To receive video, you need to enter the IP address of the machine where the video is being sent from.

## Requirements

### Running Environment

- This script has been designed to run on Red Hat Enterprise Linux (RHEL) systems.
- It is recommended to use a RHEL virtual machine (e.g., RHEL 9) for testing purposes.

### Firewall and SELinux

- To ensure the application runs smoothly, it's recommended to disable both the firewall and SELinux on your RHEL system. You can do this by running the following commands:
    ```
    systemctl stop firewalld
    setenforce 0
    ```

## Advantages

- Simplifies the process of sending and receiving live video streams.
- Provides a user-friendly interface using Tkinter.
- Easy-to-understand code structure allows customization and extension.

---

Feel free to explore and modify the code to suit your needs. This video call application can be a starting point for building more complex video communication systems or for learning how video streaming works in Python.
