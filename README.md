# NumPy_Notes — Complete NumPy Guide (Beginner → Advanced)

**NumPy_Notes** is a clean, well-organized collection of concise notes, examples, cheat-sheets and hands-on snippets to help you master NumPy for data analysis, scientific computing and machine-learning workflows.

---

## 🖼️ Visual Banner  
<!-- image inserted exactly after introduction -->
<p align="center">
  <img src="https://github.com/Ashwin18-Offcl/Numpy_Notes/blob/main/f91f299b-05b7-43d9-b54a-c47f7010e9b0.png"
       width="1200"
       height="360"
       alt="NumPy banner"/>
</p>

---

## 🚀 Quick Overview
- **What:** Notes, explained examples, practice problems, and a cheat-sheet for NumPy.  
- **Who it's for:** Data analysts, students, Python beginners, ML learners, and interview candidates.  
- **Focus:** Arrays, vectorization, broadcasting, linear algebra, random generation, reshaping, real use-cases.  

---

## 📚 Table of Contents
1. [Introduction](#-introduction)  
2. [Why NumPy?](#-why-numpy)  
3. [Repository Structure](#-repository-structure)  
4. [How to Use / Run Examples](#-how-to-use--run-examples)  
5. [Step-by-Step Topics](#-step-by-step-topics)  
6. [Selected Code Examples](#-selected-code-examples)  
7. [CheatSheet & Practice](#-cheatsheet--practice)  
8. [Contributing](#-contributing)  
9. [Tags / Topics](#-tags--topics)  
10. [License](#-license)  

---

## 🧩 Introduction
NumPy (Numerical Python) is the foundation of scientific computing in Python.  
This repository contains structured notes from **beginner to advanced**, helping you master:

- Array creation & manipulation  
- Mathematical operations  
- Broadcasting  
- Linear algebra  
- Random number generation  
- Real-world analytical tasks  

---

## ✨ Why NumPy?
- Fast, memory-efficient numeric arrays  
- Vectorized operations → no Python loops  
- Clean broadcasting rules  
- Basis for pandas, SciPy, scikit-learn, TensorFlow  

---

## 📂 Repository Structure
```
NumPy_Notes/
├─ README.md
├─ Introduction_to_NumPy.md
├─ 01_Array_Creation.md
├─ 02_Indexing_Slicing.md
├─ 03_Datatypes.md
├─ 04_Math_and_Ufuncs.md
├─ 05_Broadcasting.md
├─ 06_Random_Module.md
├─ 07_Reshape_Manipulation.md
├─ 08_Aggregation.md
├─ 09_Linear_Algebra.md
├─ 10_Practice_Problems.md
├─ Examples/
│   ├─ basics.ipynb
│   ├─ vectorization_examples.py
│   └─ matrix_ops.py
└─ CheatSheet.pdf
```

## ⚙️ How to Use / Run Examples

### **1. Clone the repository**
```bash
git clone https://github.com/Ashwin18-Offcl/Numpy_Notes.git
cd Numpy_Notes
```

### **2. Install dependencies**
```bash
pip install numpy jupyter
```

### **3. Run notebooks / python files**
```bash
jupyter notebook Examples/basics.ipynb
python Examples/vectorization_examples.py
```
## 🧭 Step-by-Step Topics

### **Beginner**
- What is NumPy?  
- Array creation (`array`, `zeros`, `ones`, `arange`, `linspace`)  
- Indexing & slicing (basic, boolean, fancy)  
- Data types & memory  

### **Intermediate**
- Vectorized operations & ufuncs  
- Broadcasting rules  
- Reshaping, flattening, stacking  
- Axis-based operations  

### **Advanced**
- Random module  
- Linear algebra (`dot`, `matmul`, `eig`, `inv`)  
- Performance tricks (views, strides)  
- Real-world array manipulation  

---

## 🧪 Selected Code Examples

### Create a NumPy array
```python
import numpy as np

arr = np.array([1, 2, 3], dtype=np.int32)
print(arr)
```

### Broadcasting example
```python
x = np.array([1, 2, 3])
y = np.array([[10],[20]])
print(x + y)
```

### Matrix multiplication
```python
A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

print(A @ B)
```

### Sliding window trick (advanced)
```python
def rolling_window(a, window):
    shape = a.shape[:-1] + (a.shape[-1] - window + 1, window)
    strides = a.strides + (a.strides[-1],)
    return np.lib.stride_tricks.as_strided(a, shape=shape, strides=strides)

arr = np.arange(10)
print(rolling_window(arr, 3))
```

## 📄 CheatSheet & Practice
- **CheatSheet.pdf** = one-page summary of all operations  
- Practice problems added from beginner → advanced  

## 🤝 Contributing
PRs are welcome!  
You can contribute:
- New examples  
- Better explanations  
- Additional practice problems  
- Bug fixes in notes  

---

## 🏷️ Tags / Topics
```
python, numpy, numpy-notes, umpy-tutorial, data-analysis, scientific-computing, cheat-sheet, learning-resources
```
