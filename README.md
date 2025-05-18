# CrystalClear
Improvements and optimizations for Rhode devices (Moto G52) and its siblings Moto G32 and G42.

## Features
- Changes to the entire Android Runtime management. This means that the entire ART of the Moto G52 has been optimized and superficially improved through AOSP Master optimizations. These optimizations vary in;
  - Dexopt profiles precisely chosen for each situation. Reduces JIT usage proportionally and increases runtime performance slightly.
  - Reduction of ART debugs/tracing/logs, this potentially reduces CPU usage by up to 1%-0.1% depending on the ROM the device is running.
  - System_Ui and SystemServer have a filter that is more beneficial for them. Improving SystemServer memory management and reducing CPU usage.
  - Instead of generic, use a more native compilation that respects the system, making ART/JIT more respectful and making the most of the Snapdragon 680, which is what the Moto G52, G32 and G42 have.
