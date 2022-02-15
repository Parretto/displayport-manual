Transmitter
===========

The Displayport TX diagram is shown in figure 1.

.. image:: ./images/dptx_diagram.svg
   :alt: DPTX Diagram
Figure 1: DisplayPort TX diagram


.. list-table:: Parameters
    :widths: 10 10 10 10
    :header-rows: 1

    * - Name
      - Type
      - Description
      - Values
    * - P_VENDOR
      - String
      - Vendor
      - Xilinx, Lattice
    * - P_BEAT
      - Integer
      - Beat value
      - 125
    * - P_LANES
      - Integer
      - Number of lanes
      - 2, 4
    * - P_SPL
      - Integer
      - Symbols per lane
      - 2
    * - P_PPC
      - Integer
      - Pixels per clock
      - 2
    * - P_BPC
      - Integer
      - Bits per component
      - 8


.. list-table:: Signals
    :widths: 10 10 10 
    :header-rows: 1
	
    * - Name
      - Clock domain 
	  - Description
    * - SYS_RST_IN
	  - SYS_CLK_IN
	  - System reset
    * - SYS_CLK_IN
	  - SYS_CLK_IN
	  - System clock (125 MHz)
