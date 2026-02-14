# 🏗️ Physical Design Made Easy

## 📘 Overview

**Physical Design Made Easy** is a beginner-friendly guide to **ASIC Physical Design**, created to simplify complex concepts using **clear explanations, minimal jargon, and real‑world analogies**. This content is designed for students and early‑career engineers who want to build a strong conceptual foundation before diving into tools and commands.

---

## 🧠 What Is Physical Design?

Physical Design is the process of transforming a logical chip design into a **physical layout that can be fabricated on silicon**. Instead of treating it as something magical or tool-heavy, this guide explains Physical Design using **common-sense thinking**, similar to how a **city is planned, powered, and connected by roads**.

---

## 🔄 Physical Design Flow (High Level)

The guide walks through the **end-to-end Physical Design flow**, helping readers build a clear mental model before exploring details:

1. 🧩 Floorplanning
2. 📍 Placement
3. ⏱️ Clock Tree Synthesis (CTS)
4. 🛣️ Routing
5. ✅ Sign-off (Timing, Crosstalk, Power Integrity)

Understanding the **order and purpose** of these steps is emphasized as the key to mastering Physical Design.

---

## 🧩 Floorplanning – The Foundation Step

Floorplanning is presented as the **most critical stage** of Physical Design, since decisions made here impact all downstream stages.

### Key Topics Covered:

### 1️⃣ Defining Core & Die

- **Die**: Entire chip boundary
- **Core**: Area where standard cells are placed
- Space between core and die is reserved for **power, IO, and routing**

### 2️⃣ Macro Placement (Pre‑Placed Cells)

- Large functional blocks like:

  - Multipliers
  - Dividers
  - Memory blocks

- Placement depends on connectivity, IO proximity, and performance needs

### 3️⃣ Decoupling Capacitors (Decaps)

- Act as **local energy storage**
- Reduce voltage drops during high switching
- Placed near macros and high‑activity regions

### 4️⃣ Power Planning ⚡

- Power is distributed using a **grid/mesh**, not a single source
- Ensures stable VDD/VSS across the chip
- Reduces IR drop and current spikes

### 5️⃣ Pin Placement 🔌

- IO pins placed along die boundary
- Positioned close to the logic they serve
- Helps reduce congestion and timing issues

### 6️⃣ Placement Blockages 🚫

- Restrict logic placement in sensitive regions like:

  - Power rings
  - Routing channels
  - IO access zones

---

## 📌 Floorplanning Summary

After floorplanning, the design has:

- Defined core and die
- Strategically placed macros
- Inserted decaps
- Planned a robust power grid
- Well-positioned pins
- Proper placement blockages

This prepares the design for **placement, routing, and final sign-off**.

---

## 🐧 Basic Linux Commands for VLSI / PD Labs

These basic Linux commands are commonly used during **VLSI, Physical Design, and EDA lab work**.

### 📁 File & Directory Management

```bash
pwd                 # Show current directory
ls                  # List files and directories
ls -l               # Detailed list
ls -a               # Show hidden files
cd <dir>            # Change directory
cd ..               # Move one level up
mkdir <dir>         # Create directory
rm -r <dir>         # Delete directory
```

### 📄 File Operations

```bash
touch file.txt      # Create empty file
cp src dest         # Copy file
mv src dest         # Move / rename file
rm file.txt         # Delete file
cat file.txt        # View file content
less file.txt       # Scroll through file
```

### 🔍 Search & Text Viewing

```bash
grep "pattern" file.txt   # Search text inside file
head file.txt              # First 10 lines
tail file.txt              # Last 10 lines
tail -f log.txt            # Live log monitoring
```

### ⚙️ Process & System Commands

```bash
top                 # View running processes
ps -ef              # List processes
df -h               # Disk usage
free -h             # Memory usage
whoami              # Current user
```

### 🧪 Commonly Used in EDA Labs

```bash
source setup.csh        # Load tool environment
chmod +x script.sh     # Make script executable
./script.sh            # Run script
clear                  # Clear terminal
```

---

## 🎯 Purpose of This Repository

- Help **beginners** understand Physical Design intuitively
- Build strong **conceptual clarity** before using EDA tools
- Serve as a **learning reference** for VLSI and ASIC aspirants

---

✨ _If you can understand how a city works, you can understand Physical Design._
