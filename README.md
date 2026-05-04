# Exam Editor

A lightweight, distraction-free plain text editor designed for exam use on managed Google Chromebooks in kiosk mode. Built for the Suffern Central School District.

## What it does

- Opens with a pre-filled student details template (Name, Grade, Teacher Name, Date, Exam)
- Full plain text editing with no spellcheck, no autocorrect, and no markdown rendering
- Proper Tab key indentation support
- Save and open files directly to a USB drive or local storage via the browser File System Access API
- Print formatting controls (font size, line height, margins)
- All menus and settings hidden behind the Esc key to keep the interface clean for students

## How to use

### For students

1. Fill in your details at the top of the editor (Name, Grade, Teacher Name, Date, Exam)
2. Click below and start writing
3. Press **Tab** to indent
4. Press **Esc** to open the menu for saving, opening, and printing

### Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `Esc` | Open / close menu |
| `Ctrl+S` | Save |
| `Ctrl+Shift+S` | Save As |
| `Ctrl+O` | Open file |
| `Ctrl+N` | New document |
| `Ctrl+P` | Print |
| `Tab` | Indent |

## Deploying on managed Chromebooks (Google Admin Console)

### 1. Host the file

This file is hosted via GitHub Pages. To use your own copy:

1. Fork or clone this repository
2. Go to **Settings → Pages** in your GitHub repo
3. Set the source to the `main` branch and `/ (root)` folder
4. Your URL will be `https://yourusername.github.io/repo-name/exam-editor.html`

### 2. Add to Google Admin Console

1. Sign in at [admin.google.com](https://admin.google.com)
2. Go to **Devices → Chrome → Apps & Extensions → Kiosks**
3. Select the relevant Organisational Unit
4. Click **+** and choose **Add by URL**
5. Paste your GitHub Pages URL
6. Optionally set it as the **Auto-launch app** so Chromebooks boot straight into the editor

### 3. Enable USB storage (if needed)

Go to **Devices → Chrome → Settings → User & Browser Settings** and make sure external storage is not blocked so students can save to a USB drive.

## Requirements

- Google Chrome 86 or later (for File System Access API)
- HTTPS hosting (required for kiosk mode)
- No internet connection required after the page has loaded

## Notes

- This is a personal project hosted independently and is not an official Suffern Central School District product
- No data is collected, transmitted, or stored anywhere — everything stays on the student's device
- The File System Access API allows saving directly to USB drives when the native file picker is used

## License

MIT — see [LICENSE](LICENSE)
