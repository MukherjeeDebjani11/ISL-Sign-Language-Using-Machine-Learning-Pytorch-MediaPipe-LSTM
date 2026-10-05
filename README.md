# ISL-Sign-Language-Using-Machine-Learning-Pytorch-MediaPipe-LSTM
## ISL (Indian Sign Language) Recognition System — In Progress

### Problem
Most sign language recognition research and datasets are ASL-centric, 
leaving Indian Sign Language (ISL) — used by millions of Deaf and 
hard-of-hearing people in India — significantly underserved. This 
project aims to translate ISL hand gestures into text in real time.

### Approach
- **Landmark extraction:** MediaPipe extracts hand-landmark coordinates 
  from each video frame, rather than classifying raw pixels — this 
  keeps the model lightweight and robust to background/lighting changes.
- **Sequence modeling:** An LSTM/GRU network processes the landmark 
  sequence over time, since signs are defined by motion, not a single frame.
- **Planned:** signer-independent evaluation (training and testing on 
  different people) to validate real-world generalization.

### Status
🚧 Actively in development. Landmark extraction pipeline is [current 
state — e.g. "working"]; classifier training is in progress.

### Challenges
[Fill in once you hit one — e.g. "visually similar handshapes causing 
misclassification" or "limited public ISL datasets requiring custom 
data collection."]

### Roadmap
- [ ] Signer-independent train/test split
- [ ] Real-time webcam inference
- [ ] Extend to continuous (sentence-level) recognition
- [ ] Deploy as a Streamlit demo
