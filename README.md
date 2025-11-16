# BB84 Quantum Key Distribution
# 🔐 BB84 Quantum Key Distribution — A Simple & Practical Simulation  
This project is a hands-on simulation of the **BB84 Quantum Key Distribution (QKD)** protocol using Qiskit.  
If you're curious about how quantum mechanics can be used to share encryption keys securely, this repository gives you a clean and easy-to-follow implementation of the entire process — from qubit preparation all the way to detecting an attacker.

---

## 🌟 Why This Project Exists  
Classical encryption depends heavily on math problems that *might* become breakable with future quantum computers.  
BB84 is different — it builds security using **physics**, not assumptions.

I built this simulation to show:  
- How a secret key can be created using qubits  
- How noise or interception affects the communication  
- How QBER (Quantum Bit Error Rate) can reveal an attacker  
- That QKD is surprisingly simple once broken down into steps  

If you're new to quantum computing, this project gives you an intuitive starting point.

---

## 🧠 What BB84 Actually Does (Explained Simply)  
Imagine two users — a **Quantum Sender** and a **Quantum Receiver** — trying to agree on a secret encryption key.

1. The Sender creates random bits.  
2. They encode each bit into a qubit using a random basis (`+` or `x`).  
3. The Receiver measures each qubit using their own random basis.  
4. Both sides publicly compare which bases they used (but not the bits!).  
5. Bits where they used the **same basis** become part of the *sifted key*.  
6. A small sample of the key is compared to calculate **QBER**.  
7. If QBER is too high, it means someone tried to intercept the qubits.

No attacker can hide, because in quantum mechanics **measuring a qubit disturbs it**.

---

## 🚀 What This Simulation Includes  
- Random qubit generation (0 or 1)  
- Random basis selection (`+` or `x`)  
- Qiskit-based qubit preparation  
- Receiver measurement  
- Optional noise and interception  
- Automatic QBER calculation  
- Cleanly formatted output summary  
- Two visual graphs:
  - **Effect of Noise on QBER**
  - **QBER With vs Without Interception**

Everything is kept readable and beginner-friendly.

---

## 📦 Repository Contents  

