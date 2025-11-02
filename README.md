# Stylophone Simulator

This project is a fully interactive, web-based simulation of the classic Stylophone handheld synthesizer, built using HTML, CSS (Tailwind), and JavaScript with the Web Audio API.

It features a realistic retro interface, a 20-key (12 bottom, 8 top) piano-style layout, and a comprehensive song player pre-loaded with over 200 songs.

## Features

* **Authentic Sound:** Uses the Web Audio API to generate a classic `sawtooth` oscillator wave, mimicking the original instrument's sound.
* **Interactive Controls:** Fully functional switches for:
    * **Power:** Turns the audio context on and off.
    * **Vibrato:** Applies an LFO (Low-Frequency Oscillator) to the pitch for a wavering effect.
    * **Tone:** Three distinct tone settings to alter the sound.
* **Realistic Keyboard:** A 20-key, two-row layout that matches the physical instrument, playable by clicking or dragging the mouse (or with touch on mobile).
* **Comprehensive Song Player:**
    * Includes a dropdown menu with **over 200 pre-loaded songs**.
    * **Song Sheet Display:** Selecting a song shows its full note sequence in a scrollable display, allowing you to learn and play it yourself.
    * **Auto-Play:** Press "Play" to have the stylophone play the selected song automatically.
    * **Visual Feedback:** The player highlights the corresponding key on the keyboard and the current note in the song sheet as it plays.
* **Advanced Playback Logic:**
    * **Slides (e.g., `8-7-6`):** Interpreted as a continuous slide, with notes played back-to-back at full tempo.
    * **Pauses (e.g., `8 7 6`):** Interpreted as distinct notes with a short 50ms pause between them.
* **Responsive & Mobile-Friendly:** The layout adapts to all screen sizes, stacking controls horizontally on mobile and moving them to the side on desktop for optimal use.

## How to Use

### Manual Play

1.  Click the **Power** switch to "ON".
2.  Click and drag your mouse (or your finger on a touch device) across the metal keys to play notes.
3.  Experiment with the **Vibrato** and **Tone** switches to change the sound.

### Song Player

1.  Click the **Power** switch to "ON".
2.  Select a song from the dropdown menu. The notes will appear in the "Song Sheet" display below.
3.  Click the **Play** button to have the song play automatically.
4.  Click the **Stop** button (or play a note manually) to stop the playback.
5.  Follow along with the highlighted notes on the song sheet to learn the song yourself!

## How to Run

This is a single-file web application. No server or build process is needed.

1.  Save the code as `stylophone.html`.
2.  Open the `stylophone.html` file in any modern web browser (like Chrome, Firefox, Safari, or Edge).
3.  Or open url from here: https://ambiguouserror.github.io/stylophone/

## Technologies Used

* **HTML5:** For the core structure of the application.
* **CSS3 & Tailwind CSS:** For all styling, layout, and responsive design.
* **JavaScript (ES6+):** For all application logic, audio generation, and player functionality.
* **Web Audio API:** For generating and controlling all audio in real-time.
