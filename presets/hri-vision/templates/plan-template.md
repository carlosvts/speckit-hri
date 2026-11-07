### Vision Pipeline *(hri-vision)*

- **Capture**: [camera, resolution, fps, exposure control; entry in the Timing Budget table]
- **Models**: [detector/estimator used, training-data provenance, published subgroup performance]
- **Confidence** *(VIS-002)*: [how confidence is produced and calibrated; threshold below which the state is unknown]
- **Frame lifecycle** *(VIS-004)*: [where frames live, when they are destroyed; guarantee of no disk/network writes]
- **Multi-person handling**: [target selection, or intended multi-person sensing and its consent mechanism]
- **Operating envelope** *(VIS-001)*: [how out-of-envelope conditions are detected (e.g., low light, no face, occlusion)]
