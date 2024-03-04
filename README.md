# M5StickC Mesh Network Lab

Welcome to the M5StickC Mesh Network Lab, where you'll dive into the fascinating world of mesh networks using the M5StickC and the Painless Mesh library. This hands-on lab session is designed to provide you with a practical understanding of how mesh networks operate and how to implement them using ESP32 devices. By following this guide, you'll learn to create a robust mesh network capable of facilitating communication between multiple M5StickC units.

## Objective

The goal of this lab is to familiarize you with mesh network principles and to give you hands-on experience in setting up a mesh network using the Painless Mesh library on M5StickC devices. You will learn to send and receive messages across the network, laying the groundwork for more complex IoT applications.

## Prerequisites

Before starting this lab, you should have:
- Basic knowledge of Arduino programming.
- M5StickC units (the entire lab session will participate in the mesh).
- A computer with Arduino IDE installed and configured for M5StickC development.

## Materials Needed

- M5StickC units
- USB cables for programming
- A stable internet connection for downloading libraries and documentation

## Setup Guide

1. **Arduino IDE Configuration**: Ensure that your Arduino IDE is set up for M5StickC development. If not, follow the instructions [here](https://docs.m5stack.com/en/quick_start/m5stickc/arduino) to configure your development environment.

2. **Install Painless Mesh Library**: Open the Arduino IDE, go to Sketch > Include Library > Manage Libraries, and search for "painlessMesh". Install the library to get started (also included in #3).

3. **Follow the Guide**: This lab session is based on the comprehensive guide provided by Random Nerd Tutorials on setting up ESP-MESH with ESP32 and ESP8266 using the painlessMesh library. Please follow the detailed steps provided in the guide to set up your mesh network: [ESP-MESH with ESP32 and ESP8266 using painlessMesh](https://randomnerdtutorials.com/esp-mesh-esp32-esp8266-painlessmesh/).

## Lab Exercises

### Basic Mesh Network Setup

- **Task 1**: Follow the guide to initialize your M5StickC devices into a mesh network. Ensure each device can join the network and communicate with others.

- **Task 2**: Modify the [example code](mesh.ino) to send a simple "Hello from M5StickC [ID]" message from each device, where [ID] is the ID to uniquely identify each M5StickC in the network.

- **Task 3**: Implement functionality to display received messages on the M5StickC's screen.

### Advanced Exercise for Testing

Once you have the basic mesh network up and running, challenge yourself with the following advanced exercise (hint are available [here](hint.md)):

- **Custom Message Routing Protocol**: Modify your code to implement a custom message routing protocol. Your protocol should include message priority handling, where messages tagged as "High Priority" are processed before others in the network queue. You can implement this in user code and do not need to modify the library directly.

  - **Step 1**: Understand the library's message handling mechanism by reviewing the Painless Mesh library source code.
  - **Step 2**: Design a simple priority scheme for messages (e.g., High, Medium, Low).
  - **Step 3**: Implement the priority handling in the message routing function.
  - **Step 4**: Test your custom protocol by sending messages with different priorities and observing the order in which they are processed. You might want to try this in your project grouping.

## Conclusion

This lab session provides a hands-on approach to understanding and implementing mesh networks using M5StickC and the Painless Mesh library. By completing this lab, you will gain valuable skills that can be applied to a wide range of IoT applications. Good luck, and have fun exploring the possibilities of mesh networks!
