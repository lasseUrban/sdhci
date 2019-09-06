# SD Host Controller Interface for Virtual Platforms

This model of an SDHCI controller is an extension for the Virtual Component Modeling Library (VCML)
by Jan Henrik Weinstock. I forked VCML from Jan and added the SDHCI model in the branch [SDHCI_dev](https://github.com/lasseUrban/vcml/tree/SDHCI_dev).

You can find the code of the model here:
[sdhci.h](https://github.com/lasseUrban/vcml/blob/SDHCI_dev/include/vcml/models/generic/sdhci.h)
[sdhci.cpp](https://github.com/lasseUrban/vcml/blob/SDHCI_dev/src/vcml/models/generic/sdhci.cpp)
[test_sdhci.cpp](https://github.com/lasseUrban/vcml/blob/SDHCI_dev/test/test_sdhci.cpp)

This version of VCML (with the SDHCI model) works with Jan's OpenRisc1000 Multicore Virtual Platform (OR1kMVP).

---
## Documentation
The SDHCI model can execute normal Peripheral Input/Output (PIO) and DMA data transactions. DMA is used by default because it is much faster than PIO. To disable DMA transactions you can use `-c system.sdhci.DMA_enabled=0`.

For more technical implementation details see [sdhci.md](https://github.com/lasseUrban/vcml/blob/SDHCI_dev/doc/models/sdhci.md) or write me an email to get insight to my bachelor thesis.

---
## About me
I am a student of Computer Engineering at RWTH Aachen University and this project is my bachelor thesis.
Feel free to test my model and please give me some feedback :-)

(lasse.urban[at]rwth-aachen.de)
