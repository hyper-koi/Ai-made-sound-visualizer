The provided HTML file is a professional-grade **real-time audio visualizer** designed with high-performance web technologies. It captures audio input (microphone or system sound) and renders dynamic graphics onto a canvas.

Here is a breakdown of its features:

### 1. Audio Processing & Integration

* **Dual Input Sources:** Users can toggle between **Microphone** (external audio) and **System/Tab** (internal computer audio).
* **Web Audio API Engine:** Uses an `AnalyserNode` with an FFT size of 2048 to process frequency data in real-time.
* **Hardware Protection:** Includes a `DynamicsCompressor` to prevent audio clipping and a built-in **Peak Limiter** labeled for 10V (matching your receiver's maximum voltage).
* **Voltage Monitor:** A visual "Peak LED" indicator turns red when the signal level is too high (above 248/255 intensity).

### 2. Visualization Modes

The engine offers three distinct visual rendering styles:

* **Orbital Core (Default):** A central pulsing sphere surrounded by a ring of orbital frequency bars that react to the beat.
* **Symmetric Bars:** A traditional bar visualizer that can be configured as a standard layout or a "Mirror Middle" alignment where bass frequencies are centered.
* **Plasma Pulse:** Soft, glowing "blobs" of light that drift across the screen and expand/contract based on specific frequency bands.

### 3. Customization & Control

* **Dynamic Color Engine:** Users can select between 1 and 10 custom colors using a color picker grid.
* **Rainbow Flow:** An automated mode that cycles the colors through the HSL spectrum at a user-defined speed.
* **Sensitivity Tuning:** A "Gain Sensitivity" slider allows users to scale the visual reaction for quiet or loud music.
* **Density Controls:** Users can adjust the number of bars (up to 512) or orbital elements (up to 360) to balance visual detail with performance.

### 4. Performance & UI Features

* **High-DPI Fixed:** The code includes a custom `resize()` function that detects the device's pixel ratio (DPR), ensuring the graphics look sharp on 4K or Retina displays.
* **FPS Limiter:** A slider allows users to cap the frame rate (up to 165 FPS) to save battery or match high-refresh-rate monitors.
* **Responsive Sidebar:** A retractable "System Engine" menu that can be hidden to provide a full-screen, immersive experience.

Would you like me to explain how to modify the code to add a new visualization mode or change the default color palette?
