# Project 3 — Procedural WebGL Shapes

This project explores basic procedural geometry generation in WebGL using custom vertex and fragment shaders. Each stage builds on the previous version, gradually introducing new rendering techniques and animation concepts.

Assignment details provided in the uploaded project description. 

---

## Project Versions

### 1. Wireframe Triangle
[My triangle](start-triangle.html)
**File:** `triangle.html`

Renders a procedurally generated equilateral triangle using:

* a vertex shader for vertex positioning
* a fragment shader for flat coloring
* the `gl.LINE_LOOP` primitive

Concepts demonstrated:

* GLSL shaders
* `gl_VertexID`
* procedural geometry generation
* basic WebGL rendering pipeline

---

### 2. Filled 10-Sided Polygon

**File:** `polygon.html`

Expands the triangle into a filled convex polygon using a triangle fan.

Features:

* uses `gl.TRIANGLE_FAN`
* dynamically controls vertex count with uniform variable `N`
* generates a decagon procedurally with trigonometry

Concepts demonstrated:

* uniform variables
* triangle fans
* procedural polygon generation
* sine/cosine vertex placement

---

### 3. Five-Pointed Star

**File:** `star.html`

Modifies the polygon logic to create a star shape by alternating vertex radii.

Features:

* alternating outer and inner vertices
* center vertex for shared triangle fan origin
* procedural star generation

Concepts demonstrated:

* conditional logic in shaders
* modulus/even-odd vertex tests
* dynamic radius calculations

---

## Concepts Covered

* WebGL rendering pipeline
* Vertex and fragment shaders
* Procedural geometry generation
* Triangle fans
* GLSL uniforms
* Animation loops
* Trigonometric vertex positioning

---

## Author

Created for CS-351 Project 3.
