# CrystalTools

**Overview**  
`CrystalTools` is a Python-based toolkit for crystallography calculations. It uses **numpy** for core computations. Optional libraries **ase** and **tkinter** are only required if you want to read CIF files to obtain lattice parameters. The toolkit is divided into three independent parts. Users can choose which part to use depending on their needs.

---

## Dependencies

- Required:
  - `numpy`
- Optional (only needed for reading CIF files):
  - `ase`
  - `tkinter`

---

## Features

### 1. Lattice parameter related calculations

- Calculate interplanar spacing  
- Calculate angles between crystallographic directions and planes  
- Convert between crystallographic directions and planes (parallel conversion)  
- Cross product calculations (plane-to-axis, axis-to-plane)  
- Plane filtering (traverse all planes within a given range, filter planes with interplanar spacing below `d_min`, or with a specific angle to a given plane)  
- Direction filtering (filter directions with a specific angle to a given direction)  

### 2. Lattice transformation calculations

- Compute plane/direction correspondence given a transformation matrix  
- Compute transformation matrix given plane or direction correspondence  
- Compute transformation matrices between three coordinate systems  

### 3. Hexagonal system three- and four-index conversion

- Convert crystallographic directions between three- and four-index notation  
- Convert crystallographic planes between three- and four-index notation  
- Compute equivalent directions in the hexagonal system  
- Compute equivalent planes in the hexagonal system  

---

## Usage Instructions

### Step 1: Determine the target module
Choose the module based on your calculation needs:

- Lattice parameter calculations → Module 1  
- Lattice transformation calculations → Module 2  
- Hexagonal three-/four-index conversion → Module 3  

### Step 2: Run the class definitions
Locate the corresponding class definition, for example:  class Lattice:

Run the class definition code and initialize the required lattice parameters if necessary.

### Step 3: Execute specific calculations

- Find the calculation feature you need.
- Enter the required input parameters according to the prompts.
- Run the method to obtain results.

### Notes

- The three parts (1, 2, 3) are independent and do not interfere with each other.
- Different functionalities within the same part can be used independently.
- If reading CIF files to obtain lattice parameters, make sure `ase` and `tkinter` are installed.
- Always run the relevant class definition before performing calculations to ensure parameters are correctly initialized.

