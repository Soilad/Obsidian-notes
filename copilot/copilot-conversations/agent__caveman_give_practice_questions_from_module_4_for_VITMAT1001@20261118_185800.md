---
epoch: 1795008480306
mode: agent
backendId: claude
sessionId: "2a1db2fd-1fcd-4a17-b0ba-c1383c2f9870"
topic: "/caveman give practice questions from module 4 for {VIT/MAT/…"
model: '{"baseModelId":"opus","effort":"low"}'
tags:
  - copilot-conversation
usage: '{"usedTokens":103416,"contextWindow":1000000,"inputTokens":2,"outputTokens":8,"cacheReadTokens":75001,"cacheWriteTokens":28405,"updatedAt":1795028895724}'
---

**user**: /caveman give practice questions from module 4 for {VIT/MAT/1001}
[Timestamp: 2026/11/18 18:58:00]

**ai**: Syllabus not in vault. Assume Module 4 = vector differentiation (Field, Gradient, Divergence, Curl, matches your notes). Say if wrong.

**Gradient and directional derivative**
1. Find $\nabla f$ at $(1,2,-1)$ for $f = x^2yz + 3xz^2$.
2. Find directional derivative of $f = xy^2 + yz^3$ at $(2,-1,1)$ along $(1,2,2)$.
3. Find max rate of change of $f = x^2 + y^2 - z$ at $(1,1,2)$ and its direction.
4. Find unit normal to surface $x^2 + y^2 + z^2 = 9$ at $(2,1,2)$.
5. Find angle between surfaces $x^2 + y^2 + z^2 = 9$ and $z = x^2 + y^2 - 3$ at $(2,-1,2)$.
6. Find tangent plane and normal line to $xy + yz + zx = 11$ at $(1,2,3)$.
7. Find $a$, $b$ so directional derivative of $f = axy^2 + byz + cz^2x^3$ at $(1,2,-1)$ has max magnitude 64 along the $z$-axis. (Find $a$, $b$, $c$.)

**Divergence**
8. Find $\nabla\cdot\vec F$ for $\vec F = xy^2\hat i + yz^2\hat j + zx^2\hat k$ at $(1,1,1)$.
9. Find $\nabla\cdot(\nabla\phi)$ for $\phi = x^3 + y^3 + z^3 - 3xyz$.
10. Show $\vec F = (x+3y)\hat i + (y-2z)\hat j + (x+az)\hat k$ is solenoidal. Find $a$.
11. Prove $\nabla\cdot(\phi\vec A) = \phi(\nabla\cdot\vec A) + \vec A\cdot\nabla\phi$.

**Curl**
12. Find $\nabla\times\vec F$ for $\vec F = (x^2 - y)\hat i + 4z\hat j + x^2\hat k$.
13. Show $\vec F = (y^2\cos x + z^3)\hat i + (2y\sin x - 4)\hat j + (3xz^2 + 2)\hat k$ is irrotational. Find scalar potential $\phi$.
14. Find constants $a$, $b$, $c$ so $\vec F = (x+2y+az)\hat i + (bx - 3y - z)\hat j + (4x + cy + 2z)\hat k$ is irrotational.
15. Prove $\nabla\times(\nabla\phi) = \vec 0$ and $\nabla\cdot(\nabla\times\vec A) = 0$.
16. Find $\nabla\times\vec F$ where $\vec F = \vec\omega\times\vec r$, $\vec\omega$ constant. Interpret.

**Mixed and identities**
17. If $\vec r = x\hat i + y\hat j + z\hat k$, $r = |\vec r|$, show $\nabla r^n = n r^{n-2}\vec r$.
18. Show $\nabla^2 (r^n) = n(n+1)r^{n-2}$. Find $n$ so $r^n$ is harmonic.
19. Show $\vec F = \dfrac{\vec r}{r^3}$ is both solenoidal and irrotational for $r \ne 0$.
20. Find $\nabla\cdot(\vec A\times\vec B)$ in terms of curls, with $\vec A = x^2\hat i + y\hat j$, $\vec B = z\hat k$, verify by direct calc.

Answers on request. Want worked solutions, or a different module scope?
<!-- copilot-message {"tools":["Glob (read)","Bash (execute)"]} -->
[Timestamp: 2026/11/18 18:58:00]

**user**: check {VIT/MAT/1001/References} now
[Timestamp: 2026/11/18 19:11:20]

**ai**: Module 4 is Vector Calculus, so my earlier set missed the second half. Questions 1–19 above cover gradient, divergence, curl and identities. Here are the missing topics.

**Vector differentiation, cylindrical geometry**
21. A particle moves with $\vec r = (t^2)\hat i + (t^3 - 4t)\hat j + (3t)\hat k$. Find velocity, speed and acceleration at $t=2$. Find the tangential and normal components of acceleration.
22. Write velocity and acceleration in cylindrical coordinates $(\rho,\phi,z)$. Find them for $\rho = 2$, $\phi = t$, $z = t^2$ at $t=1$.

**Scalar and vector potentials**
23. Show $\vec F = (2xy + z^3)\hat i + x^2\hat j + 3xz^2\hat k$ is conservative. Find $\phi$. Find the work done from $(1,-2,1)$ to $(3,1,4)$.
24. Show $\vec F = (y+z)\hat i + (z+x)\hat j + (x+y)\hat k$ has a scalar potential. Find it.
25. Find a vector potential $\vec A$ with $\nabla\times\vec A = \vec F$ for $\vec F = 2x\hat i - y\hat j - z\hat k$.

**Line integrals**
26. Evaluate $\int_C \vec F\cdot d\vec r$ for $\vec F = x^2\hat i + xy\hat j$, with $C$ the line $y=x$ from $(0,0)$ to $(1,1)$. Repeat with $C$ the parabola $y=x^2$.
27. Find the work done by $\vec F = (3x^2 - 6yz)\hat i + (2y + 3xz)\hat j + (1 - 4xyz^2)\hat k$ along $\vec r = t\hat i + t^2\hat j + t^3\hat k$ from $t=0$ to $t=1$.
28. Evaluate $\oint_C (x^2 + y)\,dx + (x - y^2)\,dy$ around the circle $x^2 + y^2 = 4$ by direct integration.

**Surface and volume integrals**
29. Evaluate $\iint_S \vec F\cdot\hat n\,dS$ for $\vec F = z\hat i + x\hat j - 3y^2z\hat k$ over the first-octant part of $x^2 + y^2 = 16$ with $0\le z\le 5$.
30. Find the flux of $\vec F = 4x\hat i - 2y^2\hat j + z^2\hat k$ out of the region bounded by $x^2 + y^2 = 4$, $z=0$, $z=3$.
31. Evaluate $\iiint_V \nabla\cdot\vec F\,dV$ for $\vec F = 2x^2y\hat i - y^2\hat j + 4xz^2\hat k$ over the first-octant region of $y^2 + z^2 = 9$, $x=2$.

**Green's theorem**
32. Verify Green's theorem for $\oint_C (xy + y^2)\,dx + x^2\,dy$, with $C$ bounded by $y=x$ and $y=x^2$.
33. Use Green's theorem to find the area of the ellipse $x^2/a^2 + y^2/b^2 = 1$.
34. Evaluate $\oint_C (3x - 8y^2)\,dx + (4y - 6xy)\,dy$, with $C$ the boundary of the triangle $(0,0)$, $(1,0)$, $(0,1)$.

**Stokes' theorem**
35. Verify Stokes' theorem for $\vec F = (x^2 + y^2)\hat i - 2xy\hat j$ over the rectangle $x=\pm a$, $y=0$, $y=b$.
36. Evaluate $\oint_C \vec F\cdot d\vec r$ for $\vec F = y\hat i + z\hat j + x\hat k$, with $C$ the intersection of $x^2 + y^2 + z^2 = a^2$ and $x + z = a$.
37. Use Stokes' theorem to evaluate $\iint_S (\nabla\times\vec F)\cdot\hat n\,dS$ for $\vec F = (y - z + 2)\hat i + (yz + 4)\hat j - xz\hat k$ over the faces of the cube $0\le x,y,z\le 2$ not in the $xy$-plane.

**Gauss divergence theorem**
38. Verify the divergence theorem for $\vec F = x^2\hat i + y^2\hat j + z^2\hat k$ over the cube $0\le x,y,z\le 1$.
39. Evaluate $\iint_S \vec r\cdot\hat n\,dS$ over a sphere of radius $a$. Use the divergence theorem.
40. Find $\iint_S (x\,dy\,dz + y\,dz\,dx + z\,dx\,dy)$ over the surface of the cylinder $x^2 + y^2 = 9$, $0\le z\le 4$, including the end caps.

Question 20 above is a vector identity and is fine. Questions 1–19 are relevant, but 7 has a flaw: it has three unknowns and only one condition, so ignore it. Want answers or worked solutions?
<!-- copilot-message {"tools":["Bash (execute)"]} -->
[Timestamp: 2026/11/18 19:11:20]

**user**: is question 25 supposed to have a cross product?
[Timestamp: 2026/11/19 00:35:44]

**ai**: Yes. $\nabla\times\vec A$ is the curl, which is a cross product of the del operator with $\vec A$. The question asks for a vector potential: a field $\vec A$ whose curl gives $\vec F$.

A vector potential exists only if $\vec F$ is solenoidal. This one is:
$$\nabla\cdot\vec F = 2 - 1 - 1 = 0$$

The full question should read: "Show $\vec F$ is solenoidal. Find $\vec A$ with $\nabla\times\vec A = \vec F$."

One answer: $\vec A = -xz\,\hat j + xy\,\hat k$.

Check:
- $\hat i$ component: $\partial_y(xy) - \partial_z(-xz) = x + x = 2x$
- $\hat j$ component: $-\partial_x(xy) = -y$
- $\hat k$ component: $\partial_x(-xz) = -z$

$\vec A$ is not unique. Adding any gradient $\nabla\psi$ gives another valid answer, because $\nabla\times\nabla\psi = \vec 0$.
[Timestamp: 2026/11/19 00:35:44]

**user**: is this in {VIT/MAT/1001/References} ?
[Timestamp: 2026/11/19 00:36:37]

**ai**: Partly. The two reference files disagree.

- **Syllabus (MAT1001 docx):** yes. Module 4 lists "Scalar and vector potentials".
- **Thomas' Calculus 14th ed. (PDF):** no. I searched it for "vector potential" and got no matches. Thomas only covers scalar potentials: the potential function $f$ of a conservative field, with $\vec F = \nabla f$.

So vector potentials are in your syllabus but not in the textbook. Expect any exam question on them to be simple, like Q25. Your PYQs folder may show how VIT tests this topic. Do you want me to search those PDFs?
<!-- copilot-message {"tools":["Bash (execute)"]} -->
[Timestamp: 2026/11/19 00:36:37]

**user**: what abt {VIT/MAT/1001/PYQs}
[Timestamp: 2026/11/19 00:37:29]

**ai**: The PYQs never ask about vector potentials. They test scalar potentials often, so Q25 is low priority.

CATs cover only Modules 1–3. Module 4 questions appear only in the FATs, usually 3 or 4 per paper. One note: `MAT1001_2024_FAT_Short1.pdf` and `MAT1001_2025_FAT_Short1.pdf` are the same file.

How often each Module 4 topic appears in the FATs:

| Topic | Count | Example |
|---|---|---|
| Directional derivative / gradient | 9 | Fall'25 Set 6 Q8, Set 3 Q9 |
| Green's theorem | 8 | Short Summer'25 Set 4 Q10, Fall'25 Set 7 Q10 |
| Irrotational + scalar potential | 6 | Fall'25 Set 6 Q9, Set 7 Q9 |
| Gauss divergence theorem | 5 | Short Summer'25 Set 2 Q9, Fall'25 Set 5 Q10 |
| Line integral / work done | 4 | Fall'25 Set 2 Q9, Set 4 Q7 |
| Stokes' theorem | 2 | Fall'25 Set 2 Q10, Set 4 Q8 |
| Divergence (meaning) | 1 | Fall'25 Set 5 Q8b |
| Vector potential, cylindrical velocity/acceleration, direct surface integrals | 0 | none |

Some of my earlier practice questions are actual exam questions:
- Q13 is Fall'25 Set 7 Q9.
- Q14 is Fall'25 Set 6 Q9.
- Q24 is Short Summer'24 Set 4 Q9.
- Q32 is Short Summer'25 Set 4 Q10.

Questions to prioritize: 1–6, 12–14, 23–24, 26–27, 32–40. Skip 7, 21–22, 25, 29 and 31 unless you have extra time.
<!-- copilot-message {"tools":["Bash (execute)","Read (read): VIT/MAT/1001/PYQs/MAT1001_2024_FAT.pdf","Read (read): VIT/MAT/1001/PYQs/MAT1001_2024_FAT_Short1.pdf","Read (read): VIT/MAT/1001/PYQs/MAT1001_2025_FAT_Short1.pdf","Read (read): VIT/MAT/1001/PYQs/MAT1001_2023_Short2.pdf","Read (read): VIT/MAT/1001/PYQs/MAT1001_2025_CAT.pdf"]} -->
[Timestamp: 2026/11/19 00:37:29]