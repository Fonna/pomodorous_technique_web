# Flip Clock & Pomodoro

## Project Overview

This is a lightweight, single-page web application that combines a **Digital Flip Clock** with a **Pomodoro Timer**. It is designed to help users track time and maintain focus using the Pomodoro technique.

The application is built entirely in a single `index.html` file, making it extremely portable and easy to run without any dependencies or build steps.

## Technologies

*   **HTML5**: Structure of the application.
*   **CSS3**: Styling for the dark theme, flip-card aesthetic, and responsive layout.
*   **JavaScript (Vanilla)**: Logic for the real-time clock, countdown timer, and Web Audio API alerts.

## Key Features

1.  **Flip Clock**:
    *   Displays current local time (Hours, Minutes, Seconds).
    *   Styled to resemble a retro mechanical flip clock.
    
2.  **Pomodoro Timer**:
    *   Standard 25-minute countdown.
    *   **Start/Pause**: Toggle the timer state.
    *   **Reset**: Return to the initial 25:00 state.
    *   **Browser Title Sync**: The page title updates with the remaining time (e.g., `(24:59) 专注中`), allowing users to check progress from other tabs.
    *   **Audio Alert**: Uses the Web Audio API to play a beep sound when the timer finishes.

## Usage

### Running the Application
Since this is a static web page, no server or installation is required.

1.  Locate the `index.html` file in the project directory.
2.  Double-click it to open it in your default web browser (Chrome, Edge, Firefox, etc.).

### Controls
*   **Clock**: Runs automatically based on your system time.
*   **Pomodoro**:
    *   Click **Start** to begin the 25-minute countdown.
    *   Click **Pause** (same button) to halt the timer.
    *   Click **Reset** to stop and revert to 25:00.

## Development

### File Structure
*   `index.html`: Contains all code (HTML, CSS, JS).

### Customization
*   **Colors**: Edit the CSS variables in the `:root` section (e.g., `--accent-color`) to change the theme.
*   **Timer Duration**: Modify the `timeLeft` variable initialization in the JavaScript section (default is `25 * 60`).

### Future Improvements (TODO)
*   Separate CSS and JS into dedicated files (`style.css`, `script.js`) for better maintainability if the project grows.
*   Implement advanced 3D CSS animations for a realistic "card flip" effect.
*   Add configuration options for custom timer durations (e.g., short/long breaks).
