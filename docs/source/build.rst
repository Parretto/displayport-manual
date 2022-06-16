Build
=====

The DP IP-cores and reference design can be downloaded from the Github repository

folder tree
|
   gateware
|
   ├── src
|
   ├── ref
|
       ├── lattice
|
       ├── kronos
|
   ├── syn
|
       ├── lattice


files::
|	gateware
|		ref
|		kronos
|	lattice
|	lfcpnx_evn
|	src
	app
	lib
	misc
	pm
	rx
	tx
	vtb
	syn
	lattice


Steps to build the reference design. 

* Change the work directory to the folder gateware/syn/lattice
* Launch the Lattice Radiant software
* Open the TCL console (View -> Show Views -> TCL Console)
* Run the project script in the TCL console by typing source ../../ref/lattice/lfcpnx_evn/build_proj.tcl

.. _Github repository: https://github.com/Parretto/DisplayPort
