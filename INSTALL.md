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

# INSTALL

## Real Genetic Algorithm Application

This guide explains how to set up, build, and run the project on your local machine.

---

## 1. Prerequisites

Ensure a **C compiler** is installed. Recommended:

- **Linux/macOS:** GCC
- **Windows:** MinGW or Visual Studio (C compiler)

Verify installation:

```bash
gcc --version
```

---

## 2. Install

Clone the repository

```bash
git clone https://github.com/Artificial-Intelligence-aka-Uniwa/Genetic-Algorithms.git
```

Navigate to project directory

```bash
cd Genetic-Algorithms/src
```

---

## 3.Run

### 3.1 Compile the Program

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

### 3.2 Run the Program

For 25 settlements:

```bash
./GA_25
```

For 12 settlements:

```bash
./GA_12
```

### 3.3 Program Execution

The GA runs for a predefined number of generations (MAXGENS).

Each generation performs:

- Selection (Roulette Wheel)
- Crossover (Single-Point)
- Mutation (Random gene replacement)
- Fitness evaluation based on Euclidean distance

The best genotype and its corresponding distance are printed to the screen and logged in a results file (results_25.txt or results_12.txt).

After all experiments, mean distances and mean best genes are displayed.

### 3.4 Configurable Parameters

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

---

## 4. Open the Documentation

1. Navigate to the `docs/` directory
2. Open the report corresponding to your preferred language:
   - English: `Genetic-Algorithms.pdf`
   - Greek: `Γενετικοί-Αλγόριθμοι.pdf`
