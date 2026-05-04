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

## Notes

- This is a personal project hosted independently and is not an official Suffern Central School District product
- No data is collected, transmitted, or stored anywhere — everything stays on the student's device
- The File System Access API allows saving directly to USB drives when the native file picker is used

## License

MIT — see [LICENSE](LICENSE)
