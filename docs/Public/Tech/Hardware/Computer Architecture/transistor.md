A *transistor* is an electrical switch in circuits. There are no moving parts. 

MOS = Metal Oxide [[semiconductor]]
There are two types of transistors: *nMOS* and *pMOS*
- nMOS
	- Connects the source and drain when $1$ is applied
	- Good at passing $0$'s but bad at passing $1$'s; pulls down (to ground) transistors
- pMOS
	- Connects the source and drain when $0$ is applied
	- Good at passing $1$'s but bad at passing $0$'s'; pulls up (to Vdd) transistors
- Use both together when building gates so we can use them on their good modes: CMOS

![[transistor.png]]
![[cmos.png]]

How they work: 
Current flows when there is an electrical difference i.e. positive to negative. When a positive voltage is applied to the gate, it attracts electrons from the substrate, making the top part of the substrate behave like it is negatively charged. Now that there is an electrical difference, the source and drain are connected, and current flows. 

![[transistor_connection.png]]
