#  Experiment 2 – Boolean Operations using LabVIEW

##  Aim
To perform Boolean operations (AND, OR, XOR, NOT, NAND) using LabVIEW.

---

##  Tools Required
- National Instruments LabVIEW (any version supporting basic VI creation)

---

##  Algorithm

| Step | Description |
|------|-------------|
| 1 | Start LabVIEW and select **Blank VI** |
| 2 | Create the **Front Panel** and **Block Diagram** panel |
| 3 | Add **Push Buttons** as inputs and **Round LEDs** as outputs on the Front Panel | 
| 4 | Place Boolean operators (`AND`, `OR`, `XOR`, `NOT`, `NAND`) in the **Block Diagram** panel |
| 5 | Wire Boolean inputs and outputs in the **Block Diagram** panel |
| 6 | Enter logic values `0` & `1` in the Front Panel and **run** the program to observe output |

---

##  Front Panel Layout
<img width="1090" height="884" alt="image" src="https://github.com/user-attachments/assets/44b214c4-5b37-4d00-b898-7ae5e9b89f16" />


<img width="607" height="554" alt="image" src="https://github.com/user-attachments/assets/16715e72-06dd-481f-8ed5-b945f22e4c93" />

---

##  Block Diagram Description

<img width="1376" height="1376" alt="image" src="https://github.com/user-attachments/assets/f15a7ad8-c23d-463b-a673-fe65567e7a4e" />


---

##  Truth Tables

### AND Gate
| X1 | X2 | Y (X1 AND X2) |
|----|----|---------------|
| 0  | 0  | 0             |
| 0  | 1  | 0             |
| 1  | 0  | 0             |
| 1  | 1  | 1             |

### OR Gate
| X1 | X2 | Y (X1 OR X2) |
|----|----|--------------|
| 0  | 0  | 0            |
| 0  | 1  | 1            |
| 1  | 0  | 1            |
| 1  | 1  | 1            |

### XOR Gate
| X1 | X2 | Y (X1 XOR X2) |
|----|----|---------------|
| 0  | 0  | 0             |
| 0  | 1  | 1             |
| 1  | 0  | 1             |
| 1  | 1  | 0             |

### NAND Gate
| X1 | X2 | Y (X1 NAND X2) |
|----|----|----------------|
| 0  | 0  | 1              |
| 0  | 1  | 1              |
| 1  | 0  | 1              |
| 1  | 1  | 0              |

### NOT Gate
| X  | Y (NOT X) |
|----|-----------|
| 0  | 1         |
| 1  | 0         |

---

##  Output

<img width="1920" height="1200" alt="VICAEXP2" src="https://github.com/user-attachments/assets/0f0a9137-eaef-4cba-97a2-b2078483949e" />

##  Result

Thus the Boolean operations (AND, OR, XOR, NOT, NAND) using LabVIEW were successfully performed and verified using truth tables.
