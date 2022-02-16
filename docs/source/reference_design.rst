Reference Design
================

The reference design is shown in figure 2.
The reference design consists of the modules DisplayPort TX (DPTX), Video Tool Box (VTB), SERDES and application. 

When the DisplayPort sink is connected, the DisplayPort TX does the link training. After a successfull training the DisplayPort TX start transmitting the incoming video data.
The Video Tool Box is a collection of video helper modules. It has a timing generator and colorbar generator. 
The application has a RISC-V processor, memory (rom and ram) and a set a peripherals. 
The RISC-V processor runs the application code and DisplayPort host driver. 
The I2C peripheral is used to configure the external reference clock synthesizer. 
The SERDES is configured through the DRP / LMMI peripheral. 
The full application or parts can be replaced by customer modules. 


.. figure:: ./images/reference_design.svg
   :alt: Reference design
   
   Figure 2: Reference design
