Transmitter
===========

The Displayport TX diagram is shown in figure 1.

.. image:: ./images/dptx_diagram.svg
   :alt: DPTX Diagram
Figure 1: DisplayPort TX diagram


Parameters
----------
+----------+---------+--------------------+-----------------+
| Name     | Type    | Description        | Values          | 
+=======+============+====================+=================+
| P_VENDOR | String  | Vendor             | Xilinx, Lattice |
+----------+---------+--------------------+-----------------+
| P_BEAT   + Integer | Beat value         | 125             |
+----------+---------+--------------------+-----------------+
| P_LANES  | Integer | Number of lanes    | 2, 4            |
+----------+---------+--------------------+-----------------+
| P_SPL    | Integer | Symbols per lane   | 2               |
+----------+---------+--------------------+-----------------+
| P_PCC    | Integer | Pixels per clock   | 2               |
+----------+---------+--------------------+-----------------+
| P_BPC    | Integer | Bits per component | 8               |
+----------+---------+--------------------+-----------------+


List Tables
-----------

.. list-table:: Parameters
    :widths: 10 5 10 50
    :header-rows: 1
    :stub-columns: 1

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

Interface
---------


.. list-table:: Interface ports
	
   * - Signal name
     - Clock domain 
	 - Description
   * - SYS_RST_IN
	 - SYS_CLK_IN
	 - System reset
   * - SYS_CLK_IN
	 - SYS_CLK_IN
	 - System clock (125 MHz)
