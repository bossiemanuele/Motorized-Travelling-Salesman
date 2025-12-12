# Min-Time Path Through 10 Cities (10×10 Square)

## Problem statement
Find the **minimum-time path** that visits **all 10 cities** inside a **10×10** square, **starting from any one of the 4 corner origins**.

- The **10 city locations have been determined randomly and available below.**

> For our proposed solution, read: **`ColonParenthesis_FinalProject.pdf`**.

---

## Origins (allowed starting points)

| Origin | 1 | 2 | 3 | 4 |
|---:|---:|---:|---:|---:|
| **x** | 0 | 10 | 10 | 0 |
| **y** | 0 | 0 | 10 | 10 |

These correspond to the four corners of the 10×10 square:
- (0, 0), (10, 0), (10, 10), (0, 10)

---

## City locations

| City | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| **x** | 8.5 | 6.2 | 3.5 | 5.1 | 4.0 | 0.8 | 2.4 | 1.2 | 1.8 | 2.4 |
| **y** | 4.2 | 0.5 | 9.0 | 9.4 | 4.9 | 4.9 | 3.4 | 9.0 | 3.7 | 1.1 |

---

## Dynamics
The vehicle is modeled using planar kinematic dynamics with heading and speed control:

\[
\dot{x} = v \cos\theta
\]

\[
\dot{y} = v \sin\theta
\]

\[
\dot{\theta} = \gamma
\]

\[
\dot{v} = a
\]

---

## Objective
Maximize \[
J = 10n - t_f
\], where:

- **`n`** = number of cities your salesman has visited

