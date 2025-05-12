# Edge Impulse Example on Seeed Studio XIAO ESP32S3 Sense

This repository is an example project using Edge Impulse with the Seeed Studio XIAO ESP32S3 Sense board.

## Hardware

* Board: [Seeed Studio XIAO ESP32S3 Sense](https://www.seeedstudio.com/XIAO-ESP32S3-Sense-p-5639.html)

## Project Structure

* `/lib/adarshk-project-1_inferencing`
  This directory contains the unmodified Edge Impulse C++ library, as originally exported from the Edge Impulse Studio. This version does not run successfully on the XIAO ESP32S3 board without changes.

* `/lib/XIAO_esp32S3_YesNo_inferencing`
  This is the library that was provided by the Seeed Studio, which was exported in Aug 2023.

Detailed steps for modifying the Edge Impulse exported library for compatibility with the ESP32S3 Sense board can be found in [this documentation](https://wiki.seeedstudio.com/tinyml_course_Key_Word_Spotting/#step-6-deploying-to-xiao-esp32s3-sense)
Change lines 42-43 to switch between both libraries.

## Development Environment

* PlatformIO Core: 6.1.18
* Platform: Espressif 32 v6.9.0
* IDE: Visual Studio Code

## Getting Started

1. Clone this repository and open it with VSCode + PlatformIO.
2. Connect your Seeed Studio XIAO ESP32S3 Sense board via USB.
3. Make sure the platformio.ini file is configured for the correct board.
4. Build and upload the project.

