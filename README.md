# Slide Notes

A distraction-free, browser-based tool for taking synchronized notes alongside PDF lecture slides. Designed for students who need speed, structure, and data safety.

## Key Features

* **Zero Install:** Runs entirely in your browser as a single HTML file.
* **Tab Isolation (Memory Only):** Data exists only in the current tab's memory. This allows you to open multiple tabs for different subjects (e.g., Physics in Tab A, History in Tab B) without them overwriting each other.
* **Dynamic View:**
    * **PDF Slides:** Displays the slide + split-screen notes.
    * **Note Slides:** Inserting a "Blank" slide automatically hides the PDF viewer, giving you full-screen space for notes.


* **Smart Navigation:**
    * **Collapsible Sidebar:** A resizeable table of contents. "Note Slides" are highlighted with a circular badge for high contrast scanning.
    * **Scroll Navigation:** Hover over the sidebar or margins and scroll to change slides. Hover over notes to scroll text.
    * **Rearrange Matrix:** A full-screen drag-and-drop grid to swap notes between slides without messing up the PDF order.


* **Dark Mode:** Press `i` to instantly invert the PDF colors for late-night studying (Classic high-contrast inversion).
* **Annotations:** Draw directly on slides with a Pen and Stroke Eraser.

## Shortcuts

| Key Combination | Action |
| --- | --- |
| **Arrow Right / Up** | Next Slide |
| **Arrow Left / Down** | Previous Slide |
| **Ctrl + Arrow** | **Force Navigation** (Works even while typing in notes) |
| **i** | **Toggle Dark Mode** (Inverts PDF colors) |
| **Ctrl + F** | Open Search / Find in Notes |
| **Esc** | Unfocus text box / Close Menus |
| **Enter** (in Header) | Save Header & Unfocus |

## Data Saving & Workflow

**⚠️ IMPORTANT:** This tool does **NOT** use Local Storage (to prevent tabs conflicting). If you close the tab without saving, data is lost.

### 1. The "Smart Save" System (Recommended)

This tool uses the modern **File System Access API** to auto-save to your disk.

1. **Start:** Click **"📂 Open (Keep Saved Link)"** to load a previous JSON file, or click **"Save As..."** to start a new one.
2. **Grant Permission:** Allow the browser to view/edit the file.
3. **Auto-Save:** Once linked, the **"Enable Auto-Save"** checkbox turns on. Your work is silently saved to that specific file on your hard drive **every 2 minutes**.
4. **Instant Save:** You can also click the **"💾 Save (Instant)"** button at any time to save without a dialog box.

### 2. Manual Export

If you are on an older browser or prefer manual control:

* Click **"Save As New File..."** to download a snapshot of your current work as a `.json` file.

### 3. Panic Recovery (RAM)

If you accidentally mass-delete text, click the **"🆘 Restore Lost Text"** button in settings. It retrieves the last large chunk of text from the tab's internal memory.

## Settings & Tools

The interface is optimized for **Grayscale / High Contrast**. Click the **Gear Icon (⚙)** to access:

### Slide Manager

* **+ Blank Before/After:** Insert a text-only slide (hides PDF view). Use this for extra notes not covered by a specific slide.
* **Shift Content ▲ / ▼:** Fixes alignment issues. If your notes are one slide behind the PDF, click **Shift Down** to push all text/drawings one slot forward.
* **♻️ Sync Slides:** Repairs the deck if the number of slides doesn't match the PDF page count.

### Rearrange Notes

* Opens a full-screen **Matrix View**.
* Drag the **bottom half** (the note) of any card and drop it onto another card to **SWAP** their text and headers.

### Drawing Tools (PDF Mode)

* **Pen:** Red annotation tool.
* **Stroke Eraser:** Deletes entire strokes/lines instantly.
* **Clear Slide:** Wipes the current slide clean.

## How to Use

1. **Launch:** Open the `.html` file in a modern browser (Chrome/Edge recommended for Auto-Save).
2. **Load:** Open Settings and select your **PDF File**.
3. **Import:** Click **"📂 Open"** to load your previous `.json` notes (if any).
4. **Auto-Save:** Ensure the **"Auto-Save"** checkbox is ticked.
5. **Work:**
* Type header/notes.
* Draw on slides.
* Press `i` for dark mode.
* Use the **Sidebar** to jump between topics.


6. **Close:** Because Auto-Save is on, you can simply close the tab when finished (though clicking Save once manually is always good practice!).