Overview
========

Introduction
------------
The DisplayPort IP-core is a DisplayPort solution for FPGA implementation. 
It has a resource optimized footprint and it is written in SystemVerilog. 
A thin host driver comes with the IP-core. The application software controls the IP-core through this driver.  

Features
--------
* DisplayPort 1.4 
* RBR, HBR, HBR2 and HBR3 line rates
* Support for 2 and 4 DP lanes
* Native video and AXI stream interfaces
* Single Stream transport mode (SST)
* Dual and quad pixels per clock

Resources
---------

Xilinx 

.. list-table:: Xilinx resources
    :widths: 10 10 10 10 10
    :header-rows: 1

    * - Module
      - LUT
      - FF
      - BRAM
      - DSP
    * - DisplayPort TX (DPTX)
      - 3541
      - 3439
      - 5
      - 0
    * - DisplayPort RX (DPRX)
      - 3997
      - 2336
      - 5
      - 0
    * - Video Toolbox (VTB)
      - 1117
      - 2614
      - 1.5
      - 2

- Device XCZU9EG
- Vivado software v2021.2
- Dual pixel datapath


Lattice

.. list-table:: Lattice resources
    :widths: 10 10 10 10 10
    :header-rows: 1

    * - Module
      - LUT
      - FF
      - EBR
      - DSP
    * - DisplayPort TX (DPTX)
      - 7361
      - 3574
      - 14
      - 0
    * - DisplayPort RX (DPRX)
      - 10094
      - 2899
      - 10
      - 0
    * - Video Toolbox (VTB)
      - 2119
      - 2384
      - 6
      - 5

- Device LFCPNX-100
- Radiant software v3.1.0.43.2
- Quad pixel datapath

