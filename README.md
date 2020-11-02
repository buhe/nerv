NERV - Naive Educational RISC-V Processor
=========================================

NERV is a very simple single-stage RV32I processor. 
It is equipped with an [RVFI interface](https://github.com/SymbioticEDA/riscv-formal/blob/master/docs/rvfi.md) and is formally verified.

![system diagram](NERV.png)

Running the simulation testbench
--------------------------------

```
git clone https://github.com/SymbioticEDA/nerv.git
cd nerv
make
```


Running the riscv-formal testbench
----------------------------------

```
git clone https://github.com/SymbioticEDA/riscv-formal.git
cd riscv-formal/cores/
git clone https://github.com/SymbioticEDA/nerv.git
cd nerv
make -j8 check
```

iCEBreaker SOC example
----------------------

See the [iCEBreaker SOC README](examples/icebreaker/README.md)
