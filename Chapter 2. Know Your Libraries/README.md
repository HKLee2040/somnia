# Know Your Libraries


## Clock

NV_CLK_gate_power: Simple clock gating. Need to disable it at FPGA design.

slcg: Slavery clock gating, the input clock bundle includes a clock to the block, a clock to the whole project, a clock from global, a signal to disable the clock gating that is from global. The output is the gated clock to the block.


## Pipe

BC_Pipe: Bubble-collapse pipe, a pipe that can bring the valid/ready signal delayed for one cycle.

IS_Pipe: Input-skid pipe, a pipe that can bring the valid/ready signal delayed for one cycle, but fix timing for ro/ri.

## RAM

nv_flopram: A flop based ram. Power: high. Speed: fast. Area: Large

nv_ram_rws: A synchronous-read, synchronous-write ram. Power: low. Speed: for small memory. Area: small.

nv_ram_rwsp: Two clocks for read, synchronous-write ram. Power: low. Speed: for large memory. Area: small.

nv_ram_rwsthp: nv_ram_rwsp with a bypass.







