# Retro-Terminal-Desktop
Author: Blaine Fisher
Version: 1.4
Date: 2025-07-071. 
Overview
  The Retro Terminal Desktop is a standalone, single-file, offline-first web application designed to mimic the aesthetic of a classic green-on-black computer terminal, inspired by interfaces like those in the Fallout series (Pip-Boy). It provides a customizable desktop environment with various widgets to enhance productivity and organization, all wrapped in a nostalgic, retro-tech theme.The entire application is self-contained in a single HTML file, requiring no internet connection, external libraries, or complex setup.
2. Features
  Retro Aesthetic: A complete green-on-black "green phosphor" theme, complete with a monospace font, text glow, and CRT scanline/flicker effects.
  Customizable Widget-Based UI:
  Draggable: Click and drag any widget by its header to move it around the desktop.
  Resizable: Click and drag the bottom-right corner of any widget to resize it.
  Collapsible: Click the [-] icon in a widget's header to collapse it, and [+] to expand it.Boundary Detection: Widgets cannot be dragged or resized outside of the visible window area, preventing them from getting lost.
  Data Persistence: The application uses the browser's local
  Storage to remember:The position, size, and collapsed/expanded state of each widget.Your to-do list items.The content of your sticky notes.
  Self-Contained & Offline-First: Everything—HTML, CSS, JavaScript, and even the font—is packed into one file. It runs directly in a web browser with no internet connection required.Dynamic Sound       Effects: Uses the Web Audio API to generate custom UI sound effects and an ambient background hum, all without needing any audio files.
Included Widgets:
  System Clock: Displays the current time and date.
  Mission Objectives (To-Do List): Add, delete, and check off tasks.
  Chronometer (Timer & Stopwatch): Includes a countdown timer and a stopwatch with lap functionality.
  Memo-Log (Reminders): Set time-based reminders that trigger a notification.
  Sticky Notes: Create multiple, independent notes.
  Arithmetic Unit (Calculator): A simple calculator for basic operations.Daily Wisdom: Shows a new quote each day.
  Date Log (Calendar): A simple monthly calendar view.
  Day Progress: A visual bar showing the percentage of the current day that has passed.
  System Status: Indicators for Network (Online/Offline) and Battery level (if supported by the browser).
3. How to Use
  Open the File: Simply open the index.html file in any modern web browser (like Chrome, Firefox, or Edge).
  Interact with Widgets:
    Move: Click and hold the header of any widget to drag it.
    Resize: Click and drag the bottom-right corner of a widget.
    Collapse/Expand: Click the [-] or [+] icon in the widget header.
    Use the Bottom Bar:
      + NOTE: Adds a new sticky note to the desktop.
      SOUND: Toggle the ambient background hum on or off. The slider controls the master volume.
      FULLSCREEN: Toggles fullscreen mode.
4. Technical Details
    Frontend: The entire application is built with vanilla HTML, CSS, and JavaScript.
    Dependencies: There are no external libraries or frameworks. This ensures maximum portability and offline functionality.
    Styling: CSS is used for the entire visual theme, including the CRT effects (::before, ::after pseudo-elements and animations).
    State Management: All user data and widget states are saved locally in the browser's local storage. This means your setup will be preserved as long as you use the same browser and don't clear its site data.
    Browser Compatibility: 
      Designed for modern desktop browsers that support:
        Web Audio API
        Resize
        Observer API
        Battery Status API (optional, for battery widget)
        Fullscreen API
