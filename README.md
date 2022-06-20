# Tail-sitter-dataset
## Introduction
This dataset is gathered for quadrotor tail-sitter UAV system identification and modeling purpose by PolyU MAV/UAV Lab.
Format: MATLAB.mat file

## Hardware
The flight data is collected on a quadrotor tail-sitter UAV based on Arkbird vtol airframe. The UAV is equipped with a 3S LiPo 2200 mAh battery, 4 Sunnysky R2207 KV2580 motors with ESCs, and two servomotors for elevon control. The flight controller is a PixRacer autopilot board which communicates with an offboard computer via Wi-Fi module ESP8266. The offboard computer is a laptop equiped with Intel Core i7 runs Ubuntu 18.04 OS. The vehicle position and orientation are measured at 200 Hz using a Vicon motion capture system with 12 cameras. The Vicon system is well calibrated before the data collection process.

## Experiment Setup
The flight data is collected using both offboard and manual flight mode. In the offboard mode, the UAV tracks the local position references sent to MAVROS topic ~setpoint_position/local. The reference trajectory contains step changes in all three directions. Three step sizes 1, 1.5, and 2 meters were desigend. In the manual mode, the UAV is operated by an expert pilot using Futaba T16SZ remote control. Three flight modes position, altitude, and stabilized were chosed to enrich the maneuvering intensity. Each experiment setup is performed three times to attenuate the influence of the random error, which results in totally 18 flight logs. The take-off and landing parts were chopped for better data quality.

## Data Process
The quadrotor states 
