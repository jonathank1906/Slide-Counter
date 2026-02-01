Here is the updated README.md including the new **Drawing, Eraser, and Slide Clearing** features.

---

# Slide Counter

## Features

* **Zero Install:** Runs entirely in your browser. (Requires internet connection on the very first load to fetch the PDF library, then works offline).
* **3 Modes:**
    * **Standard:** Slide Number + Text Header + Notes.
    * **No Slide Numbers:** Flashes visual directional cues (`>>>` or `<<<`) without numbers.
    * **PDF Slides:** Renders your actual PDF slides + Slide Number. Supports **hand-drawn annotations**.


* **Slide Annotation:** Draw directly on your slides using the Pen tool. Includes a "Stroke Eraser" to remove entire lines quickly.
* **Project File System:** Export your notes and drawings as a JSON file to backup your work or move between computers.
* **Sticky Header:** The slide indicator and PDF preview stay pinned to the top while you scroll through long notes.
* **Integrated Notepad:** A scrollable, auto-saving text area for lecture notes.

## Shortcuts

| Key Combination | Action |
| --- | --- |
| **Arrow Right / Up** | Next Slide / Pulse Forward |
| **Arrow Left / Down** | Previous Slide / Pulse Backward |
| **Ctrl + Arrow** (or Cmd) | **Force Navigation** (Works even while typing in notes) |
| **Esc** | Unfocus text box (Stop typing) |
| **Enter** (in Header) | Finish typing header |

## Data Saving & Workflow

This tool uses a two-part system to keep your data safe.

### 1. Auto-Save (Local Storage)

This runs automatically in the background. Every time you type, draw, or navigate, your progress is saved to the browser's internal memory.

**How long does it last?**

* **Forever.** It does not expire. You can restart your computer, keep it off for a month, and come back—the data will still be there.

**Will clearing "History" delete it?**

* **Safe:** If you only clear "Browsing history", your data is safe.
* **Not Safe:** If you clear "Cookies and other site data", your data will be deleted.

**Important Rules for Auto-Save:**

1. **Do not move the file:** If you move the `.html` file to a different folder, the browser treats it as a new website and your data won't appear.
2. **Do not use Incognito:** Private windows delete everything when closed.
3. **Same Browser:** Chrome data does not transfer to Firefox/Edge.

### 2. Manual Save (Project Files)

Since browsers cannot permanently store large PDF files, use this workflow for long-term projects:

* **To Save:** Click **Export Notes** in settings. This downloads a `.json` file containing all your notes, headers, and **slide drawings**.
* **To Resume:** Open the tool, load your PDF again, and then load your `.json` file. Your notes and drawings will sync up to the slides immediately.

## Settings

Click the **Gear Icon** in the top-left corner to access settings:

* **Switch Mode:** Cycle through Standard -> No Numbers -> PDF Mode.
* **Drawing Tools (PDF Mode Only):**
* **Pen:** Draw red annotations on the slide.
* **Stroke Eraser:** Click or drag over any line to delete the entire stroke.
* **Clear Slide:** Removes all drawings from the *current* slide only.


* **Load Slides (PDF):** Select your lecture slides PDF.
* **Import Notes (JSON):** Load a previously saved session.
* **Save/Export Notes:** Download your current notes and drawings as a file.
* **Number Size:** Slider to adjust the size of the corner indicator.
* **Text Size:** Slider to adjust the size of your headers and notes.
* **PDF Preview Size:** Slider to adjust the vertical height of the slide preview.
* **Reset All:** Wipes all saved data and starts fresh from Slide 0.

## How to Use

1. Save the code as an `.html` file.
2. Open the file in any modern web browser.
3. Open Settings and **Load Slides (PDF)**.
4. Switch Mode to **PDF Slides** to see the drawing tools.
5. (Optional) **Import Notes** if continuing a previous session.
6. Use the **Arrow Keys** to advance slides and type notes below.
7. When finished, click **Save/Export Notes** to keep a permanent backup.