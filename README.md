# 🔷 Hash Grid — Terminal ASCII Art in Python

A fun Python project that prints **text as large ASCII art** in the terminal using `#` and space characters — inspired by Tony Stark's iconic "Welcome, Mr. Stark" display.

```
#####   #  #  #  #  #  #  #
#        #              #
#####    #  #  #  #  #  #
#        #
#####   #  #  #  #  #  #  #
```

---

## 📁 Project Structure

| File | Description |
|---|---|
| `WELCOME_MR.STARK.py` | Prints **"WELCOME MR. STARK"** in large `#` art — the main showcase |
| `EveryLetterIncluded.py` | A **full A–Z letter dictionary** — print any word using `#` characters |
| `ThearyBehindIt.py` | Explains the **theory behind the grid** — how cells and coordinates work |
| `testgit.py` | A simple `Hello World` test file used during Git setup |

---

## 🧠 How It Works

### The Core Idea
Each letter is stored as a **2D grid (list of lists)** where:
- `#` = a filled cell (part of the letter)
- ` ` (space) = an empty cell (background)

When printed row by row, these grids form **large block letters** in the terminal.

### Example — The letter "A"
```python
'A': [
    [" ", "#", "#", "#", "#", "#", " "],
    ["#", " ", " ", " ", " ", " ", "#"],
    ["#", " ", " ", " ", " ", " ", "#"],
    ["#", "#", "#", "#", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", "#"],
    ["#", " ", " ", " ", " ", " ", "#"],
    ["#", " ", " ", " ", " ", " ", "#"],
]
```
Printed output:
```
 #####
#     #
#     #
#######
#     #
#     #
#     #
```

### Printing Logic
The grid is printed by looping **row by row (y), then column by column (x)**:
```python
for y in range(height):
    for x in range(width):
        print(cell[x][y], end='')
    print()
```
This reads each row left-to-right and moves to the next line after each row — building the letter shape line by line.

---

## 🚀 How to Run

Make sure you have **Python 3** installed.

**Print "WELCOME MR. STARK":**
```bash
python WELCOME_MR.STARK.py
```

**Print any word using the full alphabet:**
```bash
python EveryLetterIncluded.py
```

> To change the word, edit the `Sentence` list inside the file:
> ```python
> Sentence = ['H', 'E', 'L', 'L', 'O']
> ```

**See the grid coordinate theory:**
```bash
python ThearyBehindIt.py
```

---

## ✏️ Customise It

Want to print your own word? Open `EveryLetterIncluded.py` and change this line:

```python
Sentence = ['W', 'E', 'L', 'C', 'O', 'M', 'E']
```

All 26 letters (A–Z) are already defined in `letter_dict`, so you can spell out anything!

---

## 💡 What You'll Learn from This Project

- How **2D lists (grids)** work in Python
- How nested `for` loops traverse a grid row by row
- How **x/y coordinate systems** map to array indices
- A creative way to render **text as pixel art** purely in the terminal

---

## 🛠️ Requirements

- Python 3.x
- No external libraries — pure Python!

---

## 👤 Author

**Mayura Jayasinghe** — [github.com/mayura0001](https://github.com/mayura0001)

