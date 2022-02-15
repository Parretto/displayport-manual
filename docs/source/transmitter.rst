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

.. list-table:: List tables can have captions like this one.
    :widths: 10 5 10 50
    :header-rows: 1
    :stub-columns: 1

    * - List table
      - Header 1
      - Header 2
      - Header 3 long. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam sit amet mauris arcu.
    * - Stub Row 1
      - Row 1
      - Column 2
      - Column 3 long. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam sit amet mauris arcu.
    * - Stub Row 2
      - Row 2
      - Column 2
      - Column 3 long. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam sit amet mauris arcu.
    * - Stub Row 3
      - Row 3
      - Column 2
      - Column 3 long. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam sit amet mauris arcu.
      
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
