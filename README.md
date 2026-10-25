# ECG Measure

Measure a paper ECG from a photo, in the browser: intervals (HR, PR, QRS, QT/QTc), axis, age-adjusted checks for
children, screening flags and a machine-style reading, with the real tracing shown so every caliper can be verified.

**Open the app:** https://ofiras.github.io/ecg-measure/

- Runs entirely on your device (the engine is Python running in the browser via [Pyodide](https://pyodide.org)).
  Photos are never uploaded. The first visit downloads the Python runtime (~25 MB, then cached).
- **Measurement aid for clinicians - not a medical device and not a diagnosis.** Automated digitisation of a photo
  carries roughly ±10-20 ms uncertainty; verify every value on the tracing.

## Credits
- Rhythm pattern model trained on the pediatric ECG database of Zhengzhou University (figshare 27078763, CC BY 4.0).
- Pediatric normal values: Davignon et al. 1979 standards.
