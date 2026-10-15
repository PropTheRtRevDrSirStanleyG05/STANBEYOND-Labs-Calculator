# STANBEYOND-Labs-Calculator
The world's most advanced offline single-file calculator — 9 modes, symbolic calculus, 3D graphing, natural-language queries, and 118 elements in one 169KB HTML file. Zero dependencies, zero network, zero backend, fully tested.

Status: Early Alpha — results may contain mistakes. Verify important calculations.

# Use it
Open STANBEYOND Labs Calculator.html in any browser. That's it. No install, no server, no internet.

STANBEYOND Labs Calculator.html — the shipping build (168 KB)

STANBEYOND Labs Calculator.exe — Native Windows Application Wrapper (49,000 KB)

STANBEYOND Labs Calculator.apk — Native Android Application Wrapper (9,700 KB)

# Modes
| Mode | What it does |
|---|---|
| **Basic** | Arithmetic with history, keyboard support |
| **Scientific** | Full keypad: trig (deg/rad), logs, gamma, nCr/nPr, gcd/lcm, fractions |
| **Graph** | Multi-function 2D, parametric, polar, 3D wireframe + shaded solids, Mandelbrot explorer, complex domain coloring, implicit curves, vector fields, heat-equation PDE, live a/b/c sliders, inequality shading, table of values |
| **Programmer** | Exact BigInt math, HEX/DEC/OCT/BIN, bitwise ops, shifts, 8/16/32/64-bit widths |
| **Matrix** | Arithmetic up to 4×4, determinant, inverse, transpose, complex-aware eigenvalues, linear systems |
| **Complex** | Full complex arithmetic and expression evaluation |
| **Tools** | Symbolic differentiation + integration (with steps), limits, sums, Taylor series, numerical integration (adaptive Simpson), double integrals, RK4 ODE solver, root finding, nonlinear systems, Laplace transforms, polynomial roots (to degree 20), number theory (Miller–Rabin, factorization, totient, nth prime), TVM finance, distributions, statistics, regressions, curve fitting (quadratic/cubic/exponential/power + R²), vectors, unit conversion (11 categories), unit-aware arithmetic with dimensional checks, DFT, truth tables, triangle solver, date math, 118 elements + molar mass |
| **Console** | Scripting with variables, lists, ranges, loops, `map`/`filter`-style builtins, Mathematica-style `table()` |
| **Ask** | Natural language: "integrate x^2 from 0 to 1", "is 97 prime", "one plus one", "molar mass of H2O" |

# Testing
Every build ships only after the full battery re-runs green. No `eval()` anywhere — the parser is hand-written and fuzz-tested.

| Suite | Result |
|---|---|
| Engine assertions | 45 passed, 0 failed |
| UI structural checks | 58 passed, 0 failed |
| Property tests (randomized) | 62 passed, 0 failed |
| Differential fuzz (parser vs JS reference) | 2,598 comparisons, 0 mismatches |
| Minified build verification | all features present, syntax OK |

Cumulative across all development rounds: **~555+ assertions, ~11,000 fuzz comparisons, 0 failures.**

# Add to your own AI agent like Meta Muse or Manus Cue
Give the html file to your agent and ask it to "save it into your system as some sort of tool you can call through:

calc.js "expression" — evaluate anything

calc.js ask "plain english" — natural language, word numbers included

calc.js diff/integ/expand — symbolic calculus"

# License
MIT
