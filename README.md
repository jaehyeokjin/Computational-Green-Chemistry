<p align="center">
  <img src="https://jinjaehyeok.wordpress.com/wp-content/uploads/2025/08/jaehyeokjin-cc.png" alt="Computational Green Chemistry" width="500">
</p>

# An Interactive Course in Computational Green Chemistry

## About This Material
This repository contains a collection of interactive, open-source Jupyter Notebooks designed to teach and apply the core principles of green and sustainable chemistry. Developed as part of a research initiative to create modern pedagogical tools, this toolkit provides students and researchers with accessible, hands-on methods for evaluating the sustainability of chemical processes. The concepts and tools presented here were originally developed for a short lecture and interactive session series during 2024-2025.

The primary goal is to provide a hands-on, inquiry-based learning experience that bridges the gap between the theoretical principles of green chemistry and their practical, quantitative application. By using computational tools, students can directly engage with concepts like reaction efficiency, waste minimization, and energy-efficient design in a tangible way.

## Key Features
- **Interactive Calculations:** Move beyond static examples with tools that allow you to input your own reaction data.  
- **Educational Focus:** Each notebook includes clear explanations of the underlying green chemistry principles.  
- **Minimal Setup:** Run all tools directly in your browser using Binder or Google Colab—no local installation required.  
- **Open-Source:** The code is transparent and available for extension and modification by the community.  

## Lectures in Detail
Below is a summary of the each lecture available in this repository.

### 1. Atom Economy Calculator
- **Principle:** Atom Economy
- **Objective:** To calculate the theoretical efficiency of a reaction by determining what percentage of reactant atoms are incorporated into the final product. This tool introduces the foundational concept of designing waste out of a reaction at the molecular level.
- **Example:** The notebook analyzes a Wittig reaction, demonstrating how a stoichiometrically-used reagent leads to a very low atom economy (~25%), immediately flagging the process as inherently wasteful.
- **View on GitHub**: `lecture1.ipynb`  

### 2. E-Factor (Environmental Factor) Calculator
- **Principle:** Waste Prevention
- **Objective:** To quantify the actual waste generated in a process. The E-Factor provides a practical, real-world measure of efficiency by comparing the mass of waste to the mass of the product.
- **Example:** A typical lab-scale synthesis is modeled, revealing a realistic E-Factor of ~31. The analysis highlights that solvents and workup materials—not the reaction byproducts—are the largest contributors to waste.
- **View on GitHub:** `lecture2.ipynb`  

### 3. Process Mass Intensity (PMI) Calculator
- **Principle:** Waste Prevention & Systems Thinking
- **Objective:** To provide a holistic, industrial-style evaluation of a process. PMI considers the total mass of all inputs (reactants, solvents, reagents, process water) relative to the final product mass.
- **Example:** A pharmaceutical synthesis is analyzed, yielding a PMI of ~27. The powerful breakdown feature shows that solvents and water account for nearly 85% of the total process mass, demonstrating that the biggest opportunities for improvement often lie outside the core reaction.
- **View on GitHub:** `lecture3.ipynb`  

### 4. Simple Solvent Selection Guide
- **Principle:** Safer Solvents and Auxiliaries
- **Objective:** To enable proactive, data-driven decisions for solvent selection. The tool ranks common solvents based on aggregated safety, health, and environmental scores.
- **Example:** The guide categorizes solvents like ethanol as "Green," acetone as "Yellow" (use with caution), and DMF or chloroform as "Red" (problematic), empowering users to quickly identify and avoid the most hazardous options.
- **View on GitHub:** `lecture4.ipynb`  

### 5. Reagent Hazard Assessment Tool
- **Principle:** Design for Less Hazardous Chemical Syntheses
- **Objective:** To compare the inherent hazards of different synthetic routes. The tool calculates a "Total Hazard Score" based on the GHS pictograms of all starting materials.
- **Example:** A traditional oxidation using highly toxic potassium dichromate (Hazard Score: 39) is compared to a modern catalytic alternative using oxygen (Hazard Score: 14). The result is a clear, quantitative validation that the catalytic route is the inherently safer choice.
- **View on GitHub:** `lecture5.ipynb`  

### 6. MD Tutorial for Green Chemistry with Hands-on Tutorial
- **Principle:** Design for Energy Efficiency
- **Objective:** To demonstrate how advanced molecular modeling (LAMMPS) can be used to predict physical properties and guide greener choices. This module shows how to estimate the energy required to heat different solvents.
- **Example:** An MD simulation compares the energy input needed to heat acetone versus DMF. The analysis proves that acetone is ~1.6x more energy-efficient, directly correlating computational results with physical properties like boiling point and intermolecular forces. This serves as a capstone, linking molecular behavior to real-world energy consumption.
- **View on GitHub:** `lecture6.ipynb` and associated LAMMPS files (including trajectory and log files from simulations)

## Getting Started
### Option 1: Run Online (Recommended)
Click the **Binder** or **Colab** badges next to any tool above to launch it in a free, interactive, cloud-based environment. There is no need to install any software.

### Option 2: Run Locally
To run these notebooks on your own machine, you will need Python 3 and Jupyter.

Clone the repository:
```bash
git clone https://github.com/jaehyeokjin/Computational-Green-Chemistry
cd Computational-Green-Chemistry
```
Install the required packages:
```
pip install jupyterlab pandas molmass
```
Launch JupyterLab:
```
jupyter lab
```
This will open a new tab in your web browser where you can navigate to and run the notebooks.

**Future Work**
This toolkit is an ongoing project. Future directions include:
- Developing additional modules for other metrics (e.g., Reaction Mass Efficiency, Life Cycle Assessment data).
- Integrating predictive models for chemical toxicity and biodegradability.
- Building a web-based user interface using Voila or Streamlit to further increase accessibility for users without a programming background.

**License**
This project is licensed under the MIT License. See the LICENSE file for details.



