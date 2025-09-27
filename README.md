## 📅 Day 1 Progress

### Day 1
- Learned how to write and synthesize a **MUX netlist** using **Yosys**.
- Observed the **waveforms** using **GTKWave** after simulation.
- Commands used:
  ```bash
  yosys> read_verilog good_mux.v
  yosys> synth -top good_mux
  yosys> write_verilog good_mux_netlist.v
  iverilog -o mux_tb good_mux.v good_mux_tb.v
  gtkwave good_mux.vcd
