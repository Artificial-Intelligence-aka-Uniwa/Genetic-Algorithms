<p align="center">
  <img src="https://www.especial.gr/wp-content/uploads/2019/03/panepisthmio-dut-attikhs.png" alt="UNIWA" width="150"/>
</p>

<p align="center">
  <strong>UNIVERSITY OF WEST ATTICA</strong><br>
  SCHOOL OF ENGINEERING<br>
  DEPARTMENT OF COMPUTER ENGINEERING AND INFORMATICS
</p>

<p align="center">
  <a href="https://www.uniwa.gr" target="_blank">University of West Attica</a> ·
  <a href="https://ice.uniwa.gr" target="_blank">Department of Computer Engineering and Informatics</a>
</p>

<hr/>

<p align="center">
  <strong>Artificial Intelligence</strong>
</p>

<h1 align="center" style="letter-spacing: 1px;">
  Real Genetic Algorithm Application
</h1>

<p align="center">
  <strong>Vasileios Evangelos Athanasiou</strong><br>
  Student ID: 19390005
</p>

<p align="center">
  <a href="https://github.com/Ath21" target="_blank">GitHub</a> ·
  <a href="https://www.linkedin.com/in/vasilis-athanasiou-7036b53a4/" target="_blank">LinkedIn</a>
</p>

<hr/>

<p align="center">
  <strong>Supervision</strong>
</p>

<p align="center">
  Supervisor: Paris Mastorokostas, Professor
</p>
<p align="center">
  <a href="https://ice.uniwa.gr/en/emd_person/paris-mastorocostas/" target="_blank">UNIWA Profile</a>
</p>

<p align="center">
  Co-supervisor: Panagiota Tselenti, Laboratory Teaching Staff
</p>
<p align="center">
  <a href="https://ice.uniwa.gr/en/emd_person/panagiota-tselenti/" target="_blank">UNIWA Profile</a> ·
  <a href="https://www.linkedin.com/in/panagiotatselenti/" target="_blank">LinkedIn</a>
</p>

</hr>

---

<p align="center">
  Athens, January 2023
</p>

---

<p align="center">
  <img src="https://bs-uploads.toptal.io/blackfish-uploads/components/open_graph_image/8958295/og_image/optimized/0901-Genetic_Algorithms-Search_and_Optimization_by_Natural_Selection_Dan_Social-c593a24c34612eaba65058efa44e7980.png" width="250"/>
</p>

---

# README

## Real Genetic Algorithm Application

This repository contains a **Genetic Algorithm (GA) implementation** in C for solving combinatorial optimization problems involving settlements in Halkidiki.

The program simulates the GA process across a specified number of generations, using:

- **Population Initialization**
- **Selection (Roulette Wheel / Proportional)**
- **Crossover (Single-Point)**
- **Mutation (Random within bounds)**
- **Fitness Evaluation (Euclidean Distance to points)**

Two problem cases are provided:

1. **25 settlements** (`Halkidiki_25.txt`)
2. **12 settlements** (`Halkidiki_12.txt`)

The results include best solutions, fitness values, and performance metrics over multiple experiments.

---

## Table of Contents

| Section | Folder                          | Description                                                |
| ------: | ------------------------------- | ---------------------------------------------------------- |
|       1 | `assign/`                       | Assignment material for the Artificial Intelligence course |
|     1.1 | `assign/Assignment_2_AI.pdf`    | Assignment description in English                          |
|     1.2 | `assign/Εργασία_2_ΤΝ.pdf`       | Assignment description in Greek                            |
|       2 | `docs/`                         | Project documentation for genetic algorithms               |
|     2.1 | `docs/Genetic-Algorithms.pdf`   | English documentation covering genetic algorithms          |
|     2.2 | `docs/Γενετικοί-Αλγόριθμοι.pdf` | Greek documentation covering genetic algorithms            |
|       3 | `res/`                          | Execution results and outputs                              |
|     3.1 | `res/results_12.txt`            | Results for parameter set 12                               |
|     3.2 | `res/results_25.txt`            | Results for parameter set 25                               |
|       4 | `src/`                          | Source code and input files                                |
|     4.1 | `src/Halkidiki_12.txt`          | Input data for parameter set 12                            |
|     4.2 | `src/Halkidiki_25.txt`          | Input data for parameter set 25                            |
|     4.3 | `src/project_GA_new.c`          | Main C implementation of the genetic algorithm             |
|     4.4 | `src/simpleGA_new.c`            | Supporting C code for genetic algorithm                    |
|     4.5 | `src/simpleGA_new.h`            | Header file for supporting functions                       |
|     4.6 | `src/Project1.dev`              | Development or IDE project file                            |
|       5 | `README.md`                     | Repository overview and usage instructions                 |
|       6 | `INSTALL.md`                    | Usage instructions                                         |

---

## 1. Contents

1. **The World of the Problem**
   Defines coordinates of settlements and problem objectives.

2. **The Genetic Algorithm in Application for 25 Settlements**
   GA parameterization and initial population setup.

3. **The Final State of the Problem for 25 Settlements**  
   Best solutions and corresponding fitness after GA convergence.

4. **Commenting on the Genetic Algorithm Solutions**  
   Analysis of solution quality and convergence behavior.

5. **Show Paradoxical Solutions?**  
   Discussion of unexpected or non-intuitive GA outcomes.

6. **The Genetic Algorithm in Application for 12 Settlements**  
   Implementation for a smaller problem instance.

7. **The Final State of the Problem for 12 Settlements**
   GA results and performance metrics for 12 settlements.

8. **Differences in the Solutions of the Two Problems**  
   Comparative analysis highlighting insights between problem sizes.

---

## 2. Technologies Used

- **Programming Language:** C
- **Algorithm:** Genetic Algorithm (SGA)
- **Key Concepts:**
  - Population Initialization
  - Fitness Evaluation (Euclidean distance)
  - Selection (Roulette Wheel)
  - Single-Point Crossover
  - Random Mutation
- **Data Files:**
  - `Halkidiki_12.txt` – Coordinates for 12 settlements
  - `Halkidiki_25.txt` – Coordinates for 25 settlements
- **Platform:** Cross-platform C compiler (GCC recommended)
- **Output:** Log file (`results_12.txt` or `results_25.txt`) for analysis
