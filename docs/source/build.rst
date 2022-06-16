Build
=====

The DP IP-cores and reference design can be downloaded from the Github repository at https://github.com/Parretto/DisplayPort

The repository file structure is listed in figure 1.

.. figure:: ./images/repo-tree.png
   :alt: Repository tree
Figure 1: Repository tree

.. comment
.. comment	.
.. comment	└── gateware
.. comment		├── src 				- Source folder
.. comment    	│	├── app					- Application
.. comment    	│	├── lib					- Library
.. comment    	│	├── misc				- Miscellaneous
.. comment    	│	├── pm					- Policy maker
.. comment    	│	├── rx					- DP RX
.. comment    	│	├── tx					- DP TX
.. comment    	│	└── vtb					- Video toolbox
.. comment    	├── ref					- Reference folder
.. comment    	│	├── kronos				- Kronos RISC-V 
.. comment    	│	└── lattice				- Lattice
.. comment    	│   	└── lfcpnx_evn			- CertusPro-NX 
.. comment    	└── syn					- Synthesis folder
.. comment        	└── lattice				- Lattice



Kronos RISC-V
^^^^^^^^^^^^^
In the reference design the Kronos RISC-V is used as a generic application processor. 
More information about the Kronos project can be found here; https://sonalpinto.github.io/kronos/#/
|
**This processor is not part of the DP IP-core.**
It can be replaced by any hard or soft-core processor (eg. ARM, RISC-V, Microblaze, etc)
|
Before building the reference design the kronos repository needs to be downloaded. 
* Go to the folder gateware/ref and run the script 'get_kronos_repo.sh' 


Lattice CertusPro-NX reference design
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Steps to build the reference design. 

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
