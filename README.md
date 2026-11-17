# Introduction to FEM and Physics-Based ML

**Physics-Based Modeling, Simulation and Neural Networks** — lecture notes and exercises.
*Work in progress: the notes are being extended.*

A short introduction to the essentials of finite element modeling and physics-based machine learning, built on intuitive examples small enough to compute by hand. The notes are modular: the core is told in one dimension, and from there separate branches continue to two-dimensional problems, to dynamics and nonlinear problems, to physics-informed and physics-augmented neural networks, and to reduced models of whole solution fields.

**Author:** Ramses Sala

## Start here

| | |
|---|---|
| 📄 **Lecture notes** (one PDF, 96 pages) | [Essential Concepts in FEM & Physics-Based ML](1_Lecture_Notes/Essential_Concepts_FEM_and_Physics_Based_ML_Lecture_Notes.pdf) |
| 🌐 **Course website** (course map, every chapter as a web page) | [https://ramzee-s.github.io/Intro-fem-and-physics-ml/](https://ramzee-s.github.io/Intro-fem-and-physics-ml/) |
| 📓 **Exercises** (Jupyter notebooks) | [`2_Exercises/`](2_Exercises/) |

The website is this repository served by GitHub Pages. If the link does not work yet,
download the repository and open `index.html` in a browser.

## The lectures

All chapters are in the one PDF; each is also a web page.

| Part | | Title | Web page | Exercise |
|------|--|-------|----------|----------|
| I | 1 | Springs, Nodes, and the Stiffness Method | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/01_springs_and_stiffness.html) | |
| I | 2 | Elasticity as a Boundary Value Problem | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/02_boundary_value_problem.html) | [Exercise 2](2_Exercises/Exercise_2_Heat_FEM.ipynb) |
| II | 3 | Trusses in the Plane | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/03_trusses_in_the_plane.html) | |
| II | 4 | Plane Elasticity, Triangle and Quad Elements | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/04_plane_elasticity_and_triangles.html) | |
| III | 5 | Mass, Damping, and Time | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/05_mass_damping_and_time.html) | [Exercise 5](2_Exercises/Exercise_5_Dynamics.ipynb) |
| III | 6 | Nonlinear Problems and Newton's Method | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/06_nonlinear_problems.html) | [Exercise 6](2_Exercises/Exercise_6_Nonlinear.ipynb) |
| IV | A | From Curve Fitting to Neural Networks | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/A_from_curve_fitting_to_neural_networks.html) | [Exercise A](2_Exercises/Exercise_A_Regression_and_NN.ipynb) |
| IV | B | PINNs and PANNs in One Dimension | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/B_pinns_and_panns_in_one_dimension.html) | [B1](2_Exercises/Exercise_B1_PINN.ipynb) · [B2](2_Exercises/Exercise_B2_PANN.ipynb) · [B3](2_Exercises/Exercise_B3_Transfer.ipynb) |
| IV | S1 | Worked PINN Examples in One Dimension | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/S1_worked_pinn_examples.html) | [Exercise B1](2_Exercises/Exercise_B1_PINN.ipynb) |
| IV | S2 | Worked PANN Examples in One Dimension | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/S2_worked_pann_examples.html) | [Exercise B2](2_Exercises/Exercise_B2_PANN.ipynb) |
| IV | C | PINNs in Two Dimensions | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/C_pinns_in_two_dimensions.html) | |
| IV | D | Model Reduction with POD | [read](https://ramzee-s.github.io/Intro-fem-and-physics-ml/1_Lecture_Notes/html/D_model_reduction_pod.html) | [Exercise D](2_Exercises/Exercise_D_Model_Reduction.ipynb) |

Parts I to III cover the finite element method, Part IV physics-based machine learning and
model reduction. After Lecture 2 and Exercise 2 the notes split into three branches that can be read in any order: Lectures 3 and 4
(two dimensions), Lectures 5 and 6 (dynamics, nonlinear problems), and Lectures A and B
(machine learning). Lecture C needs B and 4; Lecture D needs 5 and A. The reading map at
the start of the notes shows all paths.

**Planned:** learning operators (influence lines, operator networks, attention), large
displacements and stability, and notebooks for Lectures 3, 4 and C.

## Working on the exercises

```bash
pip install -r requirements.txt
jupyter lab
```

Open a notebook from `2_Exercises/`. Read the matching chapter first; then fill in the
gaps marked `...` and run the check cell after each part. Only `numpy`, `sympy` and
`matplotlib` are needed — every network in the course is a few lines of `numpy`.

## Terms of use

Copyright © 2025 Ramses Sala. All rights reserved. You are welcome to read the material
and to use it for your own study; redistribution and modified versions need the author's
permission. See [LICENSE.md](LICENSE.md).

## About these notes

These lecture notes are based on earlier drafts that were left unfinished and set aside due to a lack of time. They were revived with extensive use of AI, in particular Claude Code with Anthropic's Claude Opus and Claude Fable models, which generated and rewrote text, figures and code under the author's direction. The author is responsible for the content, and errors may remain.

Please let me know about any errors, bugs or mistakes you find, and about suggestions for improvement or your experience of learning with these notes.

**Contact:** *[e-mail address to be added]*
