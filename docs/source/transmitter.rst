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
      - Clock 
      - Description
    * - SYS_RST_IN
      - SYS_CLK
      - System reset
    * - SYS_CLK_IN
      - SYS_CLK
      - System clock (125 MHz)
    * - HOST_IF
      - SYS_CLK
      - Host interface
    * - HOST_IRQ_OUT
      - SYS_CLK
      - Host interrupt
    * - AUX_EN_OUT
      - SYS_CLK
      - AUX channel enable
    * - AUX_TX_OUT
      - SYS_CLK
      - AUX channel transmit
    * - AUX_RX_IN
      - SYS_CLK
      - AUX channel receive
    * - HPD_IN
      - SYS_CLK
      - Hot Plug Detect
    * - HB_OUT
      - SYS_CLK
      - Heartbeat
    * - VID_CLK_IN
      - VID_CLK
      - Video clock
    * - VID_CKE_IN
      - VID_CLK
      - Video clock enable
    * - VID_VS_IN
      - VID_CLK
      - Video vertical sync
    * - VID_HS_IN
      - VID_CLK
      - Video horizontal sync
    * - VID_R_IN
      - VID_CLK
      - Video red
    * - VID_G_IN
      - VID_CLK
      - Video green
    * - VID_B_IN
      - VID_CLK
      - Video blue
    * - VID_DE_IN
      - VID_CLK
      - Video data enable

