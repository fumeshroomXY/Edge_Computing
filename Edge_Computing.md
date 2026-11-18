# Edge Computing
**Edge computing** is a computing model in which data processing is performed close to where the data is generated (the "edge" of the network), rather than sending all data to a centralized cloud or data center.

## Why Edge Computing Is Used
Traditional cloud computing follows this path:
```markdown
Device → Internet → Cloud Server → Result
```
Edge computing moves computation closer to devices:
```markdown
Device → Edge Server/Gateway → Result
             ↓
           Cloud
      (optional, later)
```
This reduces:

- **Latency** (faster response times)
- **Bandwidth usage** (less data sent to the cloud)
- **Network dependency** (can continue operating with limited connectivity)
- **Privacy risks** (sensitive data can remain local)

## Major Applications of Edge Computing

- Autonomous Vehicles
- Industrial Automation
- Smart Cameras and Video Analytics
- IoT
- Healthcare
- AR and VR
- DSP and Real-Time Signal Processing

An example of DSP in Edge Computing:
```markdown
Mic
 ↓
AEC(Acoustic Echo Cancellation)
 ↓
NS(Noise Suppression)
 ↓
AGC(Automatic Gain Control)
 ↓
Beamforming
 ↓
Wake Word
```

## Future Trend: Edge AI
The fastest-growing area is **Edge AI**, where machine-learning models run directly on local devices.

Examples:

- Smartphones running AI on NPUs
- Smart cameras with object detection
- Industrial defect inspection
- AI-powered robots

In the past, edge devices could only run:

- FFT
- FIR filters
- IIR filters
- General DSP algorithms

Now, they can run:

- CNNs (Convolutional Neural Networks)
- Transformers
- Smaller versions of LLMs


Examples include:

- Qualcomm Hexagon NPU
- Apple Neural Engine
- Intel Core Ultra NPU
- NVIDIA Jetson Orin

These chips make it possible to run AI models directly on the device itself.

- **DSP** handles the processing of signals;
- **Edge AI** interprets the content of those signals; 

Together, they form the foundation of modern edge computing systems.

A typical pipeline for a smart headset looks like this:

```markdown
Microphone
↓
DSP (AEC / NS / Beamforming)
↓
Edge AI (Keyword detection / Speech recognition)
↓
Cloud AI (Inference using complex, large-scale models)
```
