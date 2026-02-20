# 🔥 Heat Diffusion Playground (1D Heat Equation)

A tiny (but real!) scientific computing project: simulate heat spreading along a rod, **recover the material’s diffusivity** from measurements, and compute how fast the heat “fades.”

## 🚀 Run in Google Colab

**Option A — Upload**
1. Open https://colab.research.google.com  
2. **File → Upload notebook**
3. Upload `Q1_SciCodeStyle_Benchmark_GOLDEN.ipynb` (or `..._PROMPT.ipynb`)
4. **Runtime → Run all** ✅

**Option B — From GitHub**
1. Open Colab → **File → Open notebook → GitHub**
2. Paste this repo URL
3. Pick a notebook → **Runtime → Run all**

If everything is correct, you’ll see the unit tests pass at the bottom.

## 🧠 What this does 

Imagine a hot metal rod. Heat spreads out and smooths over time. That behavior is modeled by:

\[
u_t = \alpha u_{xx}
\]

This repo does three things:

- **🧊 Simulates heat diffusion** using a stable numerical method (Crank–Nicolson)
- **🕵️‍♀️ Estimates α from data** by watching temperature decay at one point over time (a mini “inverse problem”)
- **⏳ Computes half-life** of the fundamental mode: how long until the signal drops by 50%

## 📁 Files

- `Q1_SciCodeStyle_Benchmark_PROMPT.ipynb` — template version of the exercise
- `Q1_SciCodeStyle_Benchmark_GOLDEN.ipynb` — completed solution (all tests pass)

## ✨ Why it’s cool

This is the same “physics → simulation → data → inference” loop used in real modeling work (engineering, quant, scientific ML)… just in a small, clean package.

