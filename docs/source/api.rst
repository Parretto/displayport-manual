API
===

The DisplayPort IP requires a procesor to setup the core. This can be any procesor. 
A DisplayPort driver (prt_dp_drv) is provided for this task. 
This section provides information about the driver API.

* prt_dp_set_base
   description: Set the DisplayPort peripheral base address
   syntax: ``void prt_dp_set_base (prt_dp_ds_struct *dp, prt_u32 base);``

void prt_dp_init (prt_dp_ds_struct *dp, prt_u8 id);
prt_u8 prt_dp_ping (prt_dp_ds_struct *dp);
prt_u8 prt_dp_config (prt_dp_ds_struct *dp);
prt_u8 prt_dp_run (prt_dp_ds_struct *dp);
void prt_dp_status (prt_dp_ds_struct *dp);
prt_u8 prt_dptx_set_msa (prt_dp_ds_struct *dp);
void prt_dptx_set_tp (prt_dp_ds_struct *dp, prt_dp_tp_struct *tp);
prt_u8 prt_dptx_phy_test (prt_dp_ds_struct *dp, prt_u8 tps, prt_u8 volt, prt_u8 pre);
prt_u8 prt_dp_start_video (prt_dp_ds_struct *dp);
prt_u8 prt_dp_stop_video (prt_dp_ds_struct *dp);

