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
    :widths: 10 10 10 10
    :header-rows: 1

    * - Name
      - Clock 
      - Description
      - Width
    * - SYS_RST_IN
      - SYS_CLK
      - System reset
      - 1
    * - SYS_CLK_IN
      - SYS_CLK
      - System clock (125 MHz)
      - 1
    * - HOST_IF
      - SYS_CLK
      - Host interface
      - 
    * - HOST_IRQ_OUT
      - SYS_CLK
      - Host interrupt
      - 1
    * - AUX_EN_OUT
      - SYS_CLK
      - AUX channel enable
      - 1
    * - AUX_TX_OUT
      - SYS_CLK
      - AUX channel transmit
      - 1
    * - AUX_RX_IN
      - SYS_CLK
      - AUX channel receive
      - 1
    * - HPD_IN
      - SYS_CLK
      - Hot Plug Detect
      - 1
    * - HB_OUT
      - SYS_CLK
      - Heartbeat
      - 1
    * - VID_CLK_IN
      - VID_CLK
      - Video clock
      - 1
    * - VID_CKE_IN
      - VID_CLK
      - Video clock enable
      - 1
    * - VID_VS_IN
      - VID_CLK
      - Video vertical sync
      - 1
    * - VID_HS_IN
      - VID_CLK
      - Video horizontal sync
      - 1
    * - VID_R_IN
      - VID_CLK
      - Video red
      - P_PPC * P_BPC
    * - VID_G_IN
      - VID_CLK
      - Video green
      - P_PPC * P_BPC
    * - VID_B_IN
      - VID_CLK
      - Video blue
      - P_PPC * P_BPC
    * - VID_DE_IN
      - VID_CLK
      - Video data enable
      - P_PPC * P_BPC
    * - LNK_CLK_IN
      - LNK_CLK
      - Link clock
      - 1
    * - LNK_DAT_OUT
      - LNK_CLK
      - Link data
      - P_LANES * P_SPL * 11

