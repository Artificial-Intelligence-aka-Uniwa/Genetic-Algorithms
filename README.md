<p align="center">
  <img src="https://www.especial.gr/wp-content/uploads/2019/03/panepisthmio-dut-attikhs.png" alt="UNIWA" width="150"/>
</p>

<p align="center">
  <strong>UNIVERSITY OF WEST ATTICA</strong><br>
  SCHOOL OF ENGINEERING<br>
  DEPARTMENT OF COMPUTER ENGINEERING AND INFORMATICS
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
  Supervisor: Paris Mastorokostas, Professor<br>
  Co-supervisor: Panagiota Tselenti, Laboratory Teaching Staff
</p>

<p align="center">
  Athens, January 2023
</p>


---

## Overview

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

| Section | Title          | Description                                    |
|--------:|----------------|------------------------------------------------|
| assign  | Assignment     | Contains assignments and tasks                 |
| docs    | Documentation  | Project documentation, guides, and notes       |
| src     | Source Code    | All source code files and implementations      |
| res     | Results        | Output results                                 |


## Contents

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

## Technologies Used

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

---

## Installation & Run Guide

### Prerequisites

Ensure a **C compiler** is installed. Recommended:

- **Linux/macOS:** GCC  
- **Windows:** MinGW or Visual Studio (C compiler)  

Verify installation:

```bash
gcc --version
```

---

### Install
Clone the repository
```bash
git clone https://github.com/Artificial-Intelligence-aka-Uniwa/Genetic-Algorithms.git 
```
Navigate to project directory
```bash
cd Genetic-Algorithms/src
```

---

### Run

#### Compile the Program 

For 25 settlements:
```bash
gcc project_GA_new.c simpleGA_new.c -o GA_25 -lm
```
For 12 settlements:
- Update `simpleGA_new.h` to use NPOINTS=12 and CITIES_FILE="Halkidiki_12.txt"
```bash
gcc project_GA_new.c simpleGA_new.c -o GA_12 -lm
```
- `-lm` links the math library (required for sqrt, pow).

#### Run the Program

For 25 settlements:
```bash
./GA_25
```

For 12 settlements:
```bash
./GA_12
```

#### Program Execution

The GA runs for a predefined number of generations (MAXGENS).

Each generation performs:
- Selection (Roulette Wheel)
- Crossover (Single-Point)
- Mutation (Random gene replacement)
- Fitness evaluation based on Euclidean distance

The best genotype and its corresponding distance are printed to the screen and logged in a results file (results_25.txt or results_12.txt).

After all experiments, mean distances and mean best genes are displayed.

#### Configurable Parameters

Adjust GA parameters in simpleGA_new.h:

```
#define NPOINTS        25      // Number of settlements
#define POPSIZE        1000    // Population size
#define PXOVER         0.7     // Crossover probability
#define PMUTATION      0.1     // Mutation probability
#define MAXGENS        100     // Max generations
#define DISLPAYFREQ    50      // Display frequency
#define EXPERIMENTS    10      // Number of experiments
```

Change CITIES_FILE and RESULTS_FILE for 12 or 25 settlements.



