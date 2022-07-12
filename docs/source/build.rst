Build
=====

Repository
^^^^^^^^^^
The DP IP-cores and reference design can be downloaded from the `Github repository <https://github.com/Parretto/DisplayPort>`_.

The repository file structure is listed in figure 1.

.. figure:: ./images/repo-tree.png
   :align: center
   :alt: Repository tree
Figure 1: Repository tree

	.
	└── gateware
		├── src 				- Source folder
    	│	├── app					- Application
    	│	├── lib					- Library
    	│	├── misc				- Miscellaneous
    	│	├── pm					- Policy maker
    	│	├── rx					- DP RX
    	│	├── tx					- DP TX
    	│	└── vtb					- Video toolbox
    	├── ref					- Reference folder
      │  ├── kronos           - Kronos RISC-V 
    	│	├── lattice				- Lattice
    	│  │ 	└── lfcpnx_evn			- CertusPro-NX 
      │  └── xilinx           - Xilinx
      │     └── zcu102           - ZCU102
    	└── syn					- Synthesis folder
        	├── lattice				- Lattice
         └── xilinx           - Xilinx

Kronos RISC-V
^^^^^^^^^^^^^
In the reference design the Kronos RISC-V is used as a generic application processor. 
Please visit the `Kronos webpage <https://sonalpinto.github.io/kronos/#/>`_ for more information. 
Before building the reference design the kronos repository needs to be downloaded.

Go to the folder gateware/ref and run the script ``get_kronos_repo.sh``


.. note::
   This processor is not part of the DPTX IP-core or DPRX IP-core.
   It is only used to run the reference design application software.
   It can be replaced by any processor (eg. ARM, RISC-V, Microblaze, etc)


Lattice reference design
^^^^^^^^^^^^^^^^^^^^^^^^
Steps to build the Lattice CertusPro-NX reference design. 

#. Change the work directory to the folder gateware/syn/lattice
#. Launch the Lattice Radiant software
#. Open the TCL console (View -> Show Views -> TCL Console) - Figure 2
#. Build the project by typing in the TCL console; source ../../ref/lattice/lfcpnx_evn/build_proj.tcl
#. In the file list right click on the project name (dp_ref_lat_lfcpnx_evn) 
#. Select 'Regenerate All IPs...' and click OK. - Figure 3
#. Press the big green 'Run All' button on top left to start the compilation

-----

.. figure:: ./images/lat-tcl-console.png
   :align: center
   :alt: TCL-console
Figure 2: TCL-console

-----

.. figure:: ./images/lat-regenerate-ip.png
   :align: center
   :alt: Regenerate 
Figure 3: Regenerate All IPs

-----

Xilinx reference design
^^^^^^^^^^^^^^^^^^^^^^^^
Steps to build the Xilinx ZCU102 reference design. 

#. Change the work directory to the folder gateware/syn/xilinx
#. Launch the Xilinx Vivado software
#. Build the project by typing in the TCL console; source ../../ref/xilinx/zcu102/build_proj.tcl
#. After the project was build run synthesis and implementation

