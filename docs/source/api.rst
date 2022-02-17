API
===

The DisplayPort IP requires a procesor to setup the core. This can be any procesor. 
A DisplayPort driver (prt_dp_drv) is provided for this task. 
This section provides information about the driver API.

* prt_dp_set_base
   description: Set the DisplayPort peripheral base address

   syntax: ``void prt_dp_set_base (prt_dp_ds_struct *dp, prt_u32 base);``

* prt_dp_init
   description: Initialize the DisplayPort IP. 

   syntax: ``void prt_dp_init (prt_dp_ds_struct *dp, prt_u8 id);``

* prt_dp_ping
   description: Checks if the DisplayPort is alive. 

   syntax: ``prt_u8 prt_dp_ping (prt_dp_ds_struct *dp);``

* prt_dp_config
   description: 
   syntax: ``prt_u8 prt_dp_config (prt_dp_ds_struct *dp);``

* prt_dp_run
   description: Stars the DisplayPort IP.
   
   syntax: ``prt_u8 prt_dp_run (prt_dp_ds_struct *dp);``

* prt_dp_status
   description: Get the DisplayPort IP status.

   syntax: ``void prt_dp_status (prt_dp_ds_struct *dp);``

* prt_dptx_set_msa
   description: Sets the Main Stream Attributes (MSA)

   syntax: ``prt_u8 prt_dptx_set_msa (prt_dp_ds_struct *dp);``

* prt_dptx_set_tp
   description: Sets timing parameters

   syntax: ``void prt_dptx_set_tp (prt_dp_ds_struct *dp, prt_dp_tp_struct *tp);``

* prt_dp_start_video
   description: Starts video stream

   syntax: ``prt_u8 prt_dp_start_video (prt_dp_ds_struct *dp);``

* prt_dp_stop_video
   description: Stops video stream

   syntax: ``prt_u8 prt_dp_stop_video (prt_dp_ds_struct *dp);``

* prt_dptx_phy_test
   description: Forces training pattern on PHY output

   syntax: ``prt_u8 prt_dptx_phy_test (prt_dp_ds_struct *dp, prt_u8 tps, prt_u8 volt, prt_u8 pre);``

