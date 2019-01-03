## WIREDELAY

A simple wiredelay simulator used for simulating on a PCB.

Parameters

 - `Delay_rd` - propagation time to B to A
 - `Delay_g`  - propagation time to A to B

Example usage:

```
 wiredelay
	  #(.Delay_g	(TPROP_PCB),
	    .Delay_rd	(TPROP_PCB))
 u_delay_dq
	  (.A	  (dq_io[dqwd]),
	   .B	  (dq[dqwd]),
	   .reset (rst_n_i));
```
