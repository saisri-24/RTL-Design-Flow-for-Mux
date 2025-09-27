## 📅 Day 1 Progress

### Day 1
- Learned how to write and synthesize a **MUX netlist** using **Yosys**.
- Observed the **waveforms** using **GTKWave** after simulation.
- Commands used:
  ```bash
  yosys> read_verilog mux.v
  yosys> synth -top mux
  yosys> write_verilog mux_netlist.v
  iverilog -o mux_tb mux.v mux_tb.v
  vvp mux_tb
  gtkwave dump.vcd
