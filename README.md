# Digital Oscilloscope
This project implements the basic functionallities of a Digital Oscilloscope on the Terasic DE1-SoC Development Board. By using the onboard AD7928 ADC and high-speed FPGA logic, the system captures analog signals and renders them as a continuous, scalable waveform on a 640x480 VGA display. The entire project is implemented in the hardware description language, Verilog.
## Features
**Real-Time Signal Acquisition**: High-speed sampling using the 8-channel AD7928 ADC via SPI protocol.

**Hardware-Accelerated Rendering**: Custom VGA controller logic that draws a continuous trace (point-to-point interpolation) rather than simple dots.

**Dynamic Scaling**: 
Horizontal (Time-base): Adjust the sampling rate or buffer read-offset to zoom in/out on the time axis. Vertical (Voltage): Digital gain and offset adjustments to fit the signal to the screen.

**Freeze/Run Mode**: Trigger-style functionality to pause the waveform for detailed analysis.  

A video demo can be found [here](https://www.youtube.com/watch?v=ioccB-YO474&t=44s).
