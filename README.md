# timer

Minimal terminal task timer for Ubuntu/Linux.

Hotkeys:
- **Space** — pause / resume
- **r** — reset to `00:00:00`
- **q** — quit

Features:
- Shows `HH:MM:SS`
- Clears terminal on start
- Hides cursor while running (no blinking)
- No dependencies beyond standard shell utilities
- No bs

---

## Requirements

- Bash
- `git`
- `sudo` access to install into `/usr/local/bin` (optional, but recommended)

On Ubuntu you can install git with:

```bash
sudo apt update
sudo apt install git
```

---

## Install (recommended)

Clone the repo:

```bash
git clone https://github.com/JcJet/timer.git
cd timer
```

Install the script into `/usr/local/bin/timer`:

```bash
sudo install -m 0755 timer /usr/local/bin/timer
```

Run:

```bash
timer
```

---

## Run without installing

```bash
git clone https://github.com/JcJet/timer.git
cd timer
./timer
```

---

## Uninstall

```bash
sudo rm -f /usr/local/bin/timer
```

---

## Notes

- If the cursor stays hidden after a crash, reset the terminal with:

```bash
stty sane
tput cnorm 2>/dev/null || true
```
