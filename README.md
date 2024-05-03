
# RISC Pipeline Simulator (in C++)
Overview:
The RISC Pipeline Simulator is a program written in C++ that models the execution stages of a simplified RISC (Reduced Instruction Set Computing) pipeline. The program simulates the flow of instructions through different pipeline stages, including Instruction Fetch (IF), Instruction Decode (ID), Execute (EX), Memory (MEM), and Write-Back (WB).

Key Components:

Enum PipelineStage: Defines the different stages of the pipeline, allowing for easy transition between stages.
simulatePipeline Function: Implements the main simulation loop where the pipeline stages are iterated through sequentially. Each iteration simulates the processing of an instruction through the pipeline stages.
Clock Cycle Delay Simulation: Uses std::this_thread::sleep_for to introduce a delay between pipeline stages, mimicking the timing of a real pipeline execution.
Usage:

Compile and run the program to observe the sequential execution of pipeline stages.
Modify the simulation to include more detailed logic within each pipeline stage, such as instruction decoding, arithmetic operations, and data transfers.


# Cache Coherency Simulation (MESI Protocol) (in C++)
Overview:
The Cache Coherency Simulation program is a C++ implementation that simulates a simple cache system with the MESI (Modified, Exclusive, Shared, Invalid) protocol. It demonstrates cache read operations, handling cache hits and misses, and updating cache block states.

Key Components:

Enum CacheState: Represents the different states of a cache block (INVALID, SHARED, EXCLUSIVE, MODIFIED) according to the MESI protocol.
Struct CacheBlock: Defines the structure of a cache block, including fields for validity, tag, data, and state.
cacheRead Function: Simulates a cache read operation given a memory address. It checks if the data is present in the cache (cache hit) or needs to be fetched from memory (cache miss).
Usage:

Execute the program to observe cache read operations and state transitions based on cache hits and misses.
Extend the simulation to include cache write operations, eviction policies, and more complex cache coherence protocols like MSI or MOESI.
