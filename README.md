<div align="center">

<br>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:020810,30:041428,60:062040,100:0a3a6a&height=220&section=header&text=Newton%20Fractals&fontSize=68&fontColor=00d4ff&fontAlignY=40&desc=When%20a%20300-Year-Old%20Algorithm%20Meets%20the%20Complex%20Plane&descAlignY=62&descColor=1a5a7a&descSize=16&animation=fadeIn"/>

<br>

<img src="https://img.shields.io/badge/COMPLEX%20ANALYSIS-020f1f?style=for-the-badge&color=020f1f" alt=""/>
&nbsp;
<img src="https://img.shields.io/badge/ROOT%20FINDING-020f1f?style=for-the-badge&color=020f1f" alt=""/>
&nbsp;
<img src="https://img.shields.io/badge/FRACTAL%20GEOMETRY-020f1f?style=for-the-badge&color=020f1f" alt=""/>
&nbsp;
<img src="https://img.shields.io/badge/BASINS%20OF%20ATTRACTION-020f1f?style=for-the-badge&color=020f1f" alt=""/>

<br><br>

*When a 300-year-old root-finding algorithm meets the complex plane,*<br>
*the boundary between convergence and chaos is infinitely beautiful.*

<br>

[![Python](https://img.shields.io/badge/Python-3.8%2B-00d4ff?style=flat-square&logo=python&logoColor=white&labelColor=020810)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-00ffcc?style=flat-square&logo=jupyter&logoColor=white&labelColor=020810)](https://jupyter.org)
[![Kaggle](https://img.shields.io/badge/Kaggle-Live%20Notebook-00aaff?style=flat-square&logo=kaggle&logoColor=white&labelColor=020810)](https://www.kaggle.com/nachikettalekar)
[![NumPy](https://img.shields.io/badge/NumPy-Scientific-40e0d0?style=flat-square&logo=numpy&logoColor=white&labelColor=020810)](https://numpy.org)
[![License](https://img.shields.io/badge/License-MIT-1a5a7a?style=flat-square&labelColor=020810)](LICENSE)

<br>

[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/nachikettalekar/newton-fractals-the-frozen-universe)

<br>

</div>

---

## 📋 Table of Contents

| # | Section | Topic |
|:---:|:---|:---|
| 01 | ❄️ **The Mathematics** | What are Newton Fractals and why do they exist? |
| 02 | 🔵 **The Classic** | `z³ − 1 = 0` — the simplest, most iconic |
| 03 | 🌊 **Smooth Shading** | Cinematic rendering techniques |
| 04 | 🎨 **Polynomial Gallery** | Eight polynomials, eight alien universes |
| 05 | 🔬 **Deep Zoom Series** | 1000× magnification — infinite detail |
| 06 | 💎 **Nova & Halley** | Beyond Newton — other root-finding fractals |
| 07 | 🌐 **Coefficient Sweep** | 16 complex values of `c` — parameter space |
| 08 | 🗺️ **Basin Analysis** | Measuring chaos at the frontier |
| 09 | 🎭 **Grand Finale** | The ultimate showcase gallery |

---

<br>

<table><tr><td width="4px" bgcolor="#00d4ff"></td><td>
<sub><code>§ 01 · THE MATHEMATICS</code></sub><br>
<h3>❄️ What Are Newton Fractals?</h3>
</td></tr></table>

**Isaac Newton** invented his root-finding algorithm in 1669:

```
z₍ₙ₊₁₎ = zₙ − f(zₙ) / f′(zₙ)
```

Apply this to **every point in the complex plane** as a starting guess. Each point converges to one of the polynomial's roots. Color each starting point by *which root* it finds and *how fast* it gets there. The result is a **fractal** of infinite complexity.

> ❄️ **KEY INSIGHT** — The boundary between basins of attraction is **nowhere differentiable.**
> At every zoom level, it is just as complex. This is not a visual trick.
> It is a **mathematical theorem** — unavoidable for any polynomial of degree ≥ 3.

---

<br>

<table><tr><td width="4px" bgcolor="#00ffcc"></td><td>
<sub><code>§ 02 · THE CLASSIC</code></sub><br>
<h3>🔵 f(z) = z³ − 1</h3>
</td></tr></table>

Three roots. Three basins. One fractal boundary. The Newton iteration:

```
z₍ₙ₊₁₎ = (2zₙ³ + 1) / (3zₙ²)
```

The three roots of unity:
```
z₁ = 1
z₂ = e^(2πi/3)  ≈  −0.5 + 0.866i
z₃ = e^(4πi/3)  ≈  −0.5 − 0.866i
```

Every point in the plane is colored by which root it converges to. The boundary between these regions is the fractal.

---

<br>

<table><tr><td width="4px" bgcolor="#00aaff"></td><td>
<sub><code>§ 03 · RENDERING TECHNIQUES</code></sub><br>
<h3>🌊 Smooth Shading & Cinematic Rendering</h3>
</td></tr></table>

Three techniques transform a good fractal into a **cinematic** one:

| Technique | What It Does |
|:---|:---|
| **Smooth iteration count** | Eliminates harsh color bands — continuous gradient |
| **HSV coloring** | Hue = which root, Brightness = convergence speed |
| **Alpha power tuning** | Controls contrast in bright/dark regions |

The smooth iteration formula:

```
μ = i + 1 − log₂(log‖zₙ‖ / log(tol))
```

This gives a **continuous** (non-integer) count — the key to silk-smooth renders.

---

<br>

<table><tr><td width="4px" bgcolor="#40e0d0"></td><td>
<sub><code>§ 04 · POLYNOMIAL GALLERY</code></sub><br>
<h3>🎨 Eight Polynomials — Eight Alien Universes</h3>
</td></tr></table>

| Polynomial | Roots | Character |
|:---|:---:|:---|
| `z³ − 1` | 3 | Classic — the original |
| `z⁴ − 1` | 4 | Four-fold crystalline symmetry |
| `z⁵ − 1` | 5 | Five-pointed star fractal |
| `z⁶ − 1` | 6 | Snowflake — six-fold symmetry |
| `z³ − 2z + 2` | 3 | Broken symmetry — wild and asymmetric |
| `z⁴ + z³ − 1` | 4 | Alien geometry — no obvious pattern |
| `z⁵ − z + 0.5` | 5 | Near-chaotic — intricate boundary |
| `z⁸ − 1` | 8 | Eight basins — maximum complexity |

> Higher degree = more roots = more basins = **more complex boundary.**

---

<br>

<table><tr><td width="4px" bgcolor="#00d4ff"></td><td>
<sub><code>§ 05 · DEEP ZOOM</code></sub><br>
<h3>🔬 1000× Magnification — Infinite Detail</h3>
</td></tr></table>

Four progressively deeper zooms into the fractal boundary:

```
Zoom 1×     →  Full view
Zoom 10×    →  Boundary region visible
Zoom 100×   →  Deep structure emerges
Zoom 1000×  →  Same complexity as the full image
```

> 🔬 This is the mathematical definition of a fractal:
> **self-similar structure at every scale of magnification.**
> The complexity does not diminish. It is a theorem that it cannot.

---

<br>

<table><tr><td width="4px" bgcolor="#00ffcc"></td><td>
<sub><code>§ 06 · BEYOND NEWTON</code></sub><br>
<h3>💎 Nova & Halley Fractals</h3>
</td></tr></table>

Newton's method is just one of many root-finding algorithms. Each creates its own fractal:

**Nova Fractal** — Newton + perturbation constant `c`:
```
z₍ₙ₊₁₎ = zₙ − f(zₙ)/f′(zₙ) + c
```

**Halley's Method** — cubic convergence, more complex boundary:
```
z₍ₙ₊₁₎ = zₙ − 2f(zₙ)f′(zₙ) / (2[f′(zₙ)]² − f(zₙ)f″(zₙ))
```

| Method | Convergence Order | Boundary Complexity |
|:---|:---:|:---|
| Newton | Quadratic (2) | Fractal |
| Halley | Cubic (3) | More complex fractal |
| Nova | Quadratic + c | Parameter-dependent fractal |

---

<br>

<table><tr><td width="4px" bgcolor="#40e0d0"></td><td>
<sub><code>§ 07 · COEFFICIENT SWEEP</code></sub><br>
<h3>🌐 16 Complex Values of c</h3>
</td></tr></table>

Varying the coefficient `c` in `f(z) = z³ − c` across a 4×4 grid of complex values — watching the fractal morph continuously through parameter space.

This is the Newton fractal equivalent of the Mandelbrot/Julia set parameter sweep — the same polynomial family, 16 different universes.

---

<br>

<table><tr><td width="4px" bgcolor="#00aaff"></td><td>
<sub><code>§ 08 · BASIN ANALYSIS</code></sub><br>
<h3>🗺️ Measuring Chaos at the Frontier</h3>
</td></tr></table>

For `z³ − 1` with its perfect 3-fold symmetry:

```
Expected basin area:  33.333...% each
Computed basin 1:     ≈ 33.33%
Computed basin 2:     ≈ 33.33%
Computed basin 3:     ≈ 33.33%
```

> The boundary itself has area **exactly zero** — yet it is **everywhere dense**
> in the complex plane. A set of measure zero that touches every open set.

---

## ⚡ Quick Start

```bash
# Clone
git clone https://github.com/nachiket-1/newton-fractals.git
cd newton-fractals

# Install
pip install numpy matplotlib scipy jupyter

# Launch
jupyter notebook newton_fractals_kaggle.ipynb
```

**Or open live on Kaggle — no install needed:**

[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/nachikettalekar)

---

## 🔢 What Was Computed

| What | Scale |
|:---|:---|
| Polynomial variants rendered | **8 + gallery** |
| Root-finding algorithm variants | **3** (Newton, Nova, Halley) |
| Coefficient sweep panels | **16** |
| Deep zoom levels | **4** (up to 1000×) |
| Max iterations (deep zoom) | **200 per pixel** |
| Grand finale resolution | **750 × 750 per panel** |
| Notebook file size | **~51 KB** ✅ |
| Images downloaded from internet | **0** |

*Every pixel is the answer to: "which root does Newton's method converge to from here?"*

---

## ✦ The Philosophy

**Three truths Newton Fractals reveal:**

**1. Old tools contain new mysteries**
Newton invented this in 1669 to solve equations. The fractal beauty was always there, invisible — waiting 300 years for computers to make it visible.

**2. The boundary is the message**
Deep inside a basin, Newton's method is boring — it just converges. All the magic lives at the **boundary** — where the algorithm hesitates between two possible answers. This is mathematics at its most honest: showing us exactly where certainty ends.

**3. Complexity is unavoidable**
For any polynomial of degree ≥ 3, the basin boundaries are **always** fractal. Always infinitely complex. You cannot choose a polynomial that avoids this. The infinite complexity is not a quirk. It is a **theorem.**

> *"The boundary between the basins of attraction — that is where Newton's method hesitates, wavers, cannot decide. And in that indecision, it paints infinity."*

---

## 📚 Go Deeper

| Book | Author |
|:---|:---|
| **Visual Complex Analysis** | Tristan Needham |
| **The Beauty of Fractals** | Peitgen & Richter |
| **Numerical Recipes** | Press, Teukolsky et al. |
| **Complex Dynamics** | Lennart Carleson & Theodore Gamelin |

---

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0a3a6a,50:041428,100:020810&height=140&section=footer&text=Built%20with%20Python%20%C2%B7%20NumPy%20%C2%B7%20Matplotlib%20%C2%B7%20Love%20for%20Mathematics&fontSize=13&fontColor=0a3a5a&fontAlignY=60&animation=fadeIn"/>

<br>

*If this sparked something — ⭐ star the repo.*

</div>
