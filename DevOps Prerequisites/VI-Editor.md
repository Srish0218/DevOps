# Vi Editor Basics

The `vi` editor is a powerful and versatile text editor available on Unix-based systems. It has two primary modes: **Command Mode** and **Insert Mode**.

## 1. Open a File with `vi`:

```bash
vi filename
```

## 2. Command Mode and Insert Mode:

- **Command Mode:**
  - Default mode for navigation and issuing commands.
  - Press `Esc` to enter Command Mode from Insert Mode.

- **Insert Mode:**
  - Used for entering and editing text.
  - Press `i` in Command Mode to enter Insert Mode.

## 3. Move Around:

- **Navigation:**
  - Use arrow keys or `h`, `j`, `k`, `l` for left, down, up, and right movements respectively.
  
- **Word Navigation:**
  - Move to the beginning of the next word: `w`
  - Move to the beginning of the previous word: `b`

## 4. Delete a Line and Delete a Character:

- **Delete a Line:**
  - Press `dd` in Command Mode.

- **Delete a Character:**
  - Position the cursor over the character and press `x` in Command Mode.

## 5. Copy and Paste:

- **Copy (Yank):**
  - Position the cursor and press `yy` to yank a line.

- **Paste:**
  - Press `p` to paste after the cursor or `P` to paste before the cursor.

## 6. Scroll Up and Down:

- **Scroll Down:**
  - Press `Ctrl + f` to scroll forward.

- **Scroll Up:**
  - Press `Ctrl + b` to scroll backward.

## 7. Save:

- Press `:` to enter Command-Line Mode.
- Type `w` and press `Enter` to save changes.

## 8. Quit:

- Press `:` to enter Command-Line Mode.
- Type `q` and press `Enter` to quit.

## 9. Save and Quit:

- Press `:` to enter Command-Line Mode.
- Type `wq` and press `Enter` to save and quit.

## 10. Find:

- Press `/` to enter search mode.
- Type the search term and press `Enter`.
- Use `n` to find the next occurrence.

These are basic commands to get you started with the `vi` editor. There are many more advanced features and commands to explore.

Feel free to experiment and practice these commands in a file opened with `vi`.

### To practice
[KodeKloud Lab](https://kodekloud.com/topic/labs-vi-editor-2/)