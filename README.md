This is an out of order Risc-V single-processor machine.

Currently it is only in planning, but when completed, it will:

	-implement the RV32I instruction set (maybe M?) minus perhaps I/O.

	-implement basic branch target/way prediction

	-have paged virtual memory(i.e. theoretically multiple programs could be run at once).
	
	-implement a realistic memory hierarchy with TLBs, VIPT L1 data/instr caches, an L2 cache (with increased latency), a physical memory sytem (even slower), and a large disk (very slow).

	-implement precise exceptions, with a reasonable way of at least reporting them when they happen. Maybe I'll also implement a simple exception handler.

	-implement an out of order engine using a ROB and physical registers, with a commit buffer at the end.
