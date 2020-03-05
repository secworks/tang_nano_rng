# tang_nano_rng
Implementation of a high quality random number generator on the Tang Nano FPGA board


## Status
Just started. Not completed. Does not work. **Do. Not. Use.**


## Introduction
The [Tang Nano](https://tangnano.sipeed.com/en/) is a tiny, very cheap
FPGA based development board by Sipeed.

![alt text](https://www.cnx-software.com/wp-content/uploads/2019/10/Sipeed-Tang-Nano-FPGA-Board.jpg)

The board sports a GW1N-1 FPGA device from the *Gaoyun Little Bee
series*. The chip sports 1152 LUTs and  4 BlockRAMs for a total memory
of 72Kbit.

For more information about the board, see the [documentation provided by Sipeed](https://tangnano.sipeed.com/en/).

The aim of this project and repo is to implement a high quality,
cryptographically strong Random Number Generator (RNG) with an internal
noise/entropy source, conditioning, mixer and feeding a CSPRNG. Via the
API it should be possible to access raw entropy (for testing) as well as
random numbers.


## Implementation
Nothing so far. The plan is to bring in the Ring Oscillator (ROSC) based
entropy source from the [Cryptech project](https://cryptech.is/).
