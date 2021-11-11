# SD Host Controller Interface for Virtual Platforms

This model of an SDHCI controller is an extension for the Virtual Component Modeling Library (VCML)
by Jan Henrik Weinstock. It has been merged into the [VCML](https://github.com/janweinstock/vcml) in January 2020.

You can find the code of the SDHCI model here:  
[sdhci.h](https://github.com/janweinstock/vcml/tree/master/include/vcml/models/generic/sdhci.h)  
[sdhci.cpp](https://github.com/janweinstock/vcml/tree/master/src/vcml/models/generic/sdhci.cpp)  
[test_sdhci.cpp](https://github.com/janweinstock/vcml/tree/master/test/models/sdhci.cpp)

---
## Documentation
The SDHCI model can execute normal Peripheral Input/Output (PIO) and DMA data transactions. DMA is used by default because it is much faster than PIO. To disable DMA transactions you can use `-c system.sdhci.DMA_enabled=0`.

For more technical implementation details see [sdhci.md](https://github.com/janweinstock/vcml/tree/master/doc/models/sdhci.md) or have a look at my bachelor thesis uploaded in this repository.

---
## About me
I am a student of Computer Engineering at RWTH Aachen University and this project is my bachelor thesis.
Feel free to test my model and please give me some feedback :-)

(lasse.urban[at]rwth-aachen.de)
