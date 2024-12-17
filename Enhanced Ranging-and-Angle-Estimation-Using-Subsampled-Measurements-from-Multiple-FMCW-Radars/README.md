# Project Overview
This project focuses on processing FMCW radar data to estimate the range, velocity, and angle of arrival (AoA) of multiple targets. It uses subsampled radar measurements to reduce data size and improve processing efficiency. Key techniques include 2D DFT, Non-Coherent Integration, CA-CFAR Detection, and OMP-based Sparse Reconstruction.

## Files Description
# Main Script
Radar_Sim_for_cfar_n.m - Main script to simulate radar data, process it, and extract target parameters.
# Functions
# Data Generation

1.GenerateMultiple_Target_Multi_Sensor_AdcData.m - Simulates radar ADC data for multiple sensors and targets.
2.Generate_Noise.m - Adds Gaussian noise to the radar signal.
# Subsampling

3.Get_subsampled_ADC_Data.m - Performs subsampling on radar measurements.

# Signal Processing
4.find_2d_dft.m - Computes the 2D DFT of the radar signal.
5.Get_Non_Coherent_Data.m - Applies non-coherent integration to improve SNR.

# Target Detection
6.ca_cfar_2d_n.m - Detects targets using the CA-CFAR algorithm.

# Parameter Estimation
7.Range_Doppler_info_Extraction_n.m - Extracts range and velocity of detected targets.
8.Get_Angle_estimation.m - Estimates the angle of arrival (AoA).

# Sparse Reconstruction
9.OMP_FMCW_Radar.m - Performs sparse signal reconstruction using the Orthogonal Matching Pursuit (OMP) algorithm.

# Visualization
10.plot_2dft.m - Plots the 2D DFT results for range-velocity analysis.

## Steps to Run
1.Place all .m files in the same folder.
2.Open Radar_Sim_for_cfar_n.m in MATLAB.
3.Run the script:
```plaintext
run('Radar_Sim_for_cfar_n.m')
```

## Outputs
2D Range-Doppler Plots - Visualize target ranges and velocities.
CFAR Detection Results - Detect targets in noisy environments.
Target Parameters - Displays range, velocity, and AoA of detected targets.
Sparse Reconstruction Output - Reconstructed data using OMP.
## Key Features
Efficient subsampling of radar measurements.
Accurate target detection using CA-CFAR.
Improved estimation of range and angles using OMP reconstruction.
## Applications
Multi-sensor radar systems.
Real-time target detection and tracking.
Efficient signal processing for large datasets.
## Conclusion
This project demonstrates enhanced ranging and angle estimation using subsampled measurements, reducing data size while maintaining high accuracy in target detection.
