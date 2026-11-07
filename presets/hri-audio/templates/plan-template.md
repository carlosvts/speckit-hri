### Audio Pipeline *(hri-audio)*

- **Format & device**: [sample rate, buffer size, channels, backend/device]
- **Output latency**: [buffer size / sample rate + device latency; entry in the Timing Budget table]
- **Real-time constraints**: [audio callback performs no allocation, locking, or I/O]
- **Level limiting** *(AUD-001)*: [final-stage limiter/gain clamp after all mapping; calibration method for dB at the ear]
- **Smoothing** *(AUD-002)*: [parameter ramps/interpolation; max rate of change]
- **Underrun handling** *(AUD-003)*: [detection (xrun counter), fallback (fade to silence), recovery]
- **Mapping** *(AUD-005)*: [which sound parameters encode which state, with ranges; how confidence modulates mapping strength]
