# Pac-Man (Assembly)

This is a Pac-Man–style game written entirely in **x86 Assembly** using the Irvine32 library for Windows.  
It runs in the console and features classic Pac-Man gameplay, menus, levels, scores, and sound effects.

## 🕹️ Features
- Console-based Pac-Man clone.
- Multiple levels with walls, coins, power-ups, and fruits.
- Player movement with WASD keys.
- Pause and resume gameplay.
- High score tracking via a text file (`score.txt`).
- Colorful ASCII menus and game screens.
- Background sound effects and music using `PlaySound`.

## 🛠️ Technologies / Dependencies
- **x86 Assembly (MASM)**
- **Irvine32** library (for console I/O, colors, cursor control, etc.)
- **Winmm.lib** and **Shell32.lib** (for playing sounds and shell operations)
- **Windows** platform (tested with MASM32 / Visual Studio setup)

## 📂 Important Files
- `Source.asm` — main game code.
- `pacman.bmp` / `pacman.jpg` — graphics references.
- `video.mp4` — video reference.
- `score.txt` — stores high scores.
- `Pac-Man intro music.wav`, `1.wav`, `pacman_death.wav` — sound effects.

## ▶️ How to Build & Run
1. Make sure you have MASM32 or Visual Studio with MASM support installed.
2. Include `Irvine32.inc` and link `Irvine32.lib`, `Winmm.lib`, and `Shell32.lib`.
3. Assemble and link:
   ```bash
   ml /c /coff Source.asm
   link /subsystem:console Source.obj Irvine32.lib Winmm.lib Shell32.lib
````

4. Run the executable in a Windows console:

   ```bash
   Source.exe
   ```

## 🎮 Controls

* **W** — Move Up
* **S** — Move Down
* **A** — Move Left
* **D** — Move Right
* **P** — Pause
* **R** — Resume
* **B** — Back to Menu
* **X** — Exit Game

## 📜 License

This project is for educational purposes. You may modify and distribute it with proper credit.

---

Enjoy retro Pac-Man vibes in pure assembly!

```

Would you like me to include **screenshot placeholders** (so when you add images to the repo, they’ll show up in the README)?
```
