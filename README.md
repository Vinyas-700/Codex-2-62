📂 Dataset & Model Reference
🔹 Voice Stress Dataset (for calibration reference)
While the demo runs locally (no external model calls), the following open datasets inspired the feature extraction logic:
RAVDESS – Ryerson Audio-Visual Database of Emotional Speech and Song
SAVEE – Surrey Audio-Visual Expressed Emotion
CREMA-D – Crowd-Sourced Emotional Speech Dataset
These datasets were analyzed offline to determine typical acoustic patterns of stress vs calm speech (pitch shift, centroid increase, high-frequency ratios).

🔹 Ambient Dataset
Brightness and noise thresholds are heuristic — tuned using environmental samples collected across:
Indoor (office, classroom, home)
Outdoor (daylight, shaded, nighttime)
Enabling light-level classification: Dark, Dim, Normal, Bright, Very Bright.

🔹 1. Voice Feature Extraction
Real-time processing with Web Audio API:
FFT (1024-point) for spectral features
Autocorrelation for pitch
ZCR for signal activity
All computed in 200ms intervals for smooth feedback.

🔹 2. Stress Index Computation
0.3 * VolumeVariation + 0.4 * FrequencyRatio + 0.3 * EnergyLevel
+ 0.3 * (VSA Deviation)

🔹 3. Optimization
Calibration phase (3s) establishes individual baselines.
Stress deviation computed using z-score normalization for personal sensitivity.
Efficient DOM updates via batched rendering (reduces CPU/GPU load).

🔹 4. Device Compatibility
Optimized for modern browsers supporting:
getUserMedia
AudioContext
Canvas API

🔒 Privacy & Permissions

✅ Local Processing Only:
All audio and video data are analyzed in your browser — no data is sent to a server.

✅ Ephemeral Data:
Microphone and camera access stop immediately when you click “Stop Analysis.”
No data is stored beyond the current session.

✅ User Data Safety:
User registration info (name, email, contact) is stored securely using localStorage and can be cleared anytime via Logout.

✅ Permissions:
Microphone and camera prompts appear only when analysis starts.
Declining permissions safely disables related features without breaking the app.
