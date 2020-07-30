# Firmware Binary File Size Tracking

This project is an an attempt to analyze, track, and manage firmware binary size over time. The planned output will be something like a combination of [this article from Memfault](https://interrupt.memfault.com/blog/code-size-deltas) and [this visualization from mbed](https://armmbed.github.io/mbed-os-linker-report/).

## Supported Compilers

Initial support will be for EWAVR (IAR for AVR) since that is my use case. But the analysis/parsing part will communicate with the output part by means of a well defined JSON schema. The schema will is located [here](schema/binary-analysis.schema.json). Support for elf files via `nm`/`objdump` should come very soon after IAR support is finished.
