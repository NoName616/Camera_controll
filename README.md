# Optris Pi 640 Camera Control

A Rust application for controlling the Optris Pi 640 thermal camera with an egui-based graphical interface.

## Overview

This project provides a Rust-based interface for the Optris Pi 640 thermal camera. It uses egui for the graphical user interface and Windows API through FFI to communicate with the camera hardware via the ImagerIPC2 library.

## Features

- Camera connection and disconnection
- Thermal image capture
- Camera parameter configuration (temperature range, emissivity, distance)
- Thermal image visualization
- Cross-platform GUI using egui

## Dependencies

- Rust 2021 edition
- egui and eframe for GUI
- Windows SDK for Windows API access
- ImagerIPC2 library from Optris SDK

## Setup

1. Ensure you have Rust installed (version 2021 edition or later)
2. Install the Optris camera drivers and SDK
3. Place the ImagerIPC2.dll in a location accessible to the application
4. Clone this repository
5. Build the project with `cargo build`

## Usage

1. Connect your Optris Pi 640 camera
2. Run the application with `cargo run`
3. Use the GUI to connect to the camera
4. Capture and visualize thermal images
5. Adjust camera parameters as needed

## Project Structure

- `src/main.rs`: Application entry point
- `src/app.rs`: egui application implementation
- `src/camera.rs`: Camera abstraction layer
- `src/ffi.rs`: FFI bindings for ImagerIPC2 library
- `src/utils.rs`: Utility functions for image processing

## License

This project is licensed under the MIT License - see the LICENSE file for details.