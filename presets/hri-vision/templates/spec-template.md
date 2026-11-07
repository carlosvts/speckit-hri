### Vision Sensing *(hri-vision)*

<!-- Anything inferred from images is an estimate with confidence, never a certainty. -->

- **People in frame**: [Who is expected in view. State whether sensing more than one person is
  intended by design; if yes, how every sensed person is informed and consents; if no, how
  non-target people are ignored]
- **Deployment context**: [Where this runs. If emotions/intentions are inferred in a workplace or
  education setting in the EU, flag it: the EU AI Act prohibits this except for medical or safety
  reasons]
- **VIS-001** *(III, VI)*: [Capture conditions the feature must handle, e.g., lighting range,
  distance, head pose, occlusion; behavior outside them, e.g., "state becomes unknown"]
- **VIS-002** *(III)*: [What is inferred from images and how uncertainty is expressed, e.g.,
  "estimated engagement with confidence; below [threshold] the state is unknown, never guessed"]
- **VIS-003** *(I, VIII)*: [Fairness, e.g., "detection and inference perform comparably across
  skin tone, age and gender within the target group; how this is checked"]
- **VIS-004** *(II)*: [Camera privacy, e.g., "frames are processed in memory and never stored or
  transmitted; a visible indicator shows when the camera is active"]
