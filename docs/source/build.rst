Build
=====

The DP IP-cores and reference design can be downloaded from the Github repository at https://github.com/Parretto/DisplayPort

file tree:: text
   gateware
   ├── src
   ├── ref
       ├── lattice
       ├── kronos
	├── syn
		├── lattice


Lattice CertusPro-NX reference design
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Steps to build the reference design. 

#. Change the work directory to the folder gateware/syn/lattice
#. Launch the Lattice Radiant software
#. Open the TCL console (View -> Show Views -> TCL Console)
.. figure:: ./images/lat-tcl-console.png

#. Build the project by typing in the TCL console; source ../../ref/lattice/lfcpnx_evn/build_proj.tcl
#. In the file list right click on the project (dp_ref_lat_lfcpnx_evn) 
#. Select 'Regenerate All IPs...' and click OK.
.. figure:: ./images/lat-regenerate-ip.png

#. Click on 'Run All' to start the compilation
