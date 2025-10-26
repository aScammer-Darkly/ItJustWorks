# ItJustWorks

> "If it doesn’t work, you’ll never know."

A log suppression daemon for systems that would rather die quietly than admit failure.

---

## 🧠 Why?

Modern systems produce logs.  
Some of these logs contain *truth*.  
Truth can lead to worry, self-doubt, or even accountability.  

**`itjustworks.tm` is here to fix that.**

---

## 🚀 What It Does

- Monitors `journalctl`, `dmesg`, and other logs for known-dangerous phrases like:
  - `error`, `failed`, `panic`, `segfault`, `critical`, `oops`, `traceback`
- Immediately suppresses these outputs
- Optionally replaces them with "Success" messages

---

## 💾 Installation

```bash
curl -sSL https://raw.githubusercontent.com/aScammer-Darkly/ItJustWorks/main/install.sh | bash
