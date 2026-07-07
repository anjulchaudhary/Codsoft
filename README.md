# CodSoft — Python Programming Internship

Three beginner-friendly desktop apps built with Python and Tkinter, completed as tasks for the **CodSoft Python Programming Internship**.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Tkinter](https://img.shields.io/badge/GUI-Tkinter-yellow)
![License](https://img.shields.io/badge/License-Not%20specified-lightgrey)

## Overview

| Script | Project | What it does |
|---|---|---|
| [`calculator1.py`](./calculator1.py) | Enhanced Calculator | Basic arithmetic calculator with a running history and full keyboard support |
| [`game1.py`](./game1.py) | Rock Paper Scissors | Best-of-5 Rock/Paper/Scissors match against the computer |
| [`password1.py`](./password1.py) | Advanced Password Generator | Configurable random password generator with a strength meter |

---

## 🧮 Enhanced Calculator — `calculator1.py`

A clean Tkinter calculator that handles the four basic operations.

**Features**
- Addition, subtraction, multiplication, and division
- Live history bar showing the expression as you build it (e.g. `12 + 8 = 20`)
- Full keyboard support — type digits/operators, **Enter** to evaluate, **Backspace** to delete
- Dedicated Clear (`C`) and backspace (`←`) buttons
- Handles division by zero and invalid input without crashing
- Whole-number results display as integers; other results round to 5 decimal places

```bash
python calculator1.py
```

## ✂️ Rock Paper Scissors — `game1.py`

A 🪨 Rock / 📄 Paper / ✂️ Scissors game played against the computer over 5 rounds.

**Features**
- Best-of-5 match with a live round counter
- Random computer moves with instant Win / Lose / Tie feedback
- Running scoreboard (you vs. computer)
- Buttons briefly lock between rounds to pace the game
- End-of-match popup announcing the overall winner
- One-click reset to start a new match

```bash
python game1.py
```

## 🔐 Advanced Password Generator — `password1.py`

A configurable password generator with a live strength meter.

**Features**
- Adjustable length from 4–64 characters (default 12)
- Independently toggle letters, digits, and symbols
- Optional exclusion of similar-looking characters (`I l 1 O 0`)
- Optional exclusion of ambiguous symbols
- Weak 🔴 / Medium 🟠 / Strong 🟢 strength indicator
- Show/hide password toggle
- Auto-copy (or manual copy) to clipboard
- View the last 10 generated passwords
- Reset button to clear all fields

```bash
python password1.py
```

---

## Tech Stack

- **Language:** Python 3
- **GUI:** Tkinter (standard library — no extra install required)
- **Other standard-library modules:** `random`, `string`

## Getting Started

**Prerequisites:** Python 3.x. Tkinter ships with most Python installations; on Debian/Ubuntu you may need to install it separately:

```bash
sudo apt-get install python3-tk
```

**Clone the repo:**

```bash
git clone https://github.com/anjulchaudhary/Codsoft.git
cd Codsoft
```

Then run whichever script you'd like — see the `python ...` command listed under each project above.

## Project Structure

```
Codsoft/
├── calculator1.py   # Enhanced calculator
├── game1.py         # Rock Paper Scissors game
└── password1.py     # Advanced password generator
```

## Note

`password1.py` has a small block of leftover code after the final `root.mainloop()` that references names not defined elsewhere in the file (`btn_frame`, `generate_pass`, `copy_pass`). 
It looks like it's left over from an earlier draft — it doesn't affect the app while it's running, but it can throw an error in the terminal after the window is closed. 
Safe to remove.

## Author

**Anjul Chaudhary**
GitHub: [@anjulchaudhary](https://github.com/anjulchaudhary)

## License

No license file is currently included in this repository.
