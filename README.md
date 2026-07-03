# SmartMirror
A standalone, low-power fitness monitoring system built on a **Raspberry Pi Zero 2 W** (ARM Cortex-A53) that analyzes exercise form in real-time.

## Hardware Components
- Raspberry Pi Zero 2 W (512MB RAM limit)
-Arducam OV5647 5MP Sensor (connected via MIPI CSI-2 bus)
- 5" LCD Panel (connected via GPIO/HDMI interface)
  
## Optimization Highlights for 512MB RAM
- Configured Pi OS to boot without a desktop environment, saving ~150MB of RAM.
- CSI frames downsampled to 480p to lower CPU compute on the Cortex-A53 cores.
- Integrated the lightweight inference model to achieve ~15 FPS.

