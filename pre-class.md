# **Pre-Class Study: Getting Ready for NumPy**

Welcome to Lesson 1.6\! In this session, we transition from SQL databases to the "engine" of Python data science: **NumPy**.

## **1\. Setup & Installation**

To ensure we can start coding immediately, please complete these steps before class. We recommend using `conda` to manage your environment.

### **A. Environment Preparation**

1. Open your terminal (or Anaconda Prompt).  
2. Create or activate your course environment:

```
# If you have the environment.yml file:
conda env create -f environment.yml

# Or activate your existing environment:
conda activate pds
```

### **B. Installing NumPy**

If NumPy is not already in your environment, you can install it using one of the following commands:

* **Using Conda (Recommended):**

```
conda install numpy
```

*   
  **Using Pip:**

```
pip install numpy
```

### **C. VSCode Configuration**

1. Open VSCode and verify the **Jupyter** extension is installed.  
2. Open the provided `numpy_workshop.ipynb`.  
3. In the top right, click **Select Kernel** and choose your `pds` environment.

## **2\. Prerequisites Recap**

We assume you are comfortable with:

* **Python Lists:** Understanding how to store and access elements in `[1, 2, 3]`.  
* **Basic Math:** Operators like `*`, `/`, and `**`.  
* **VSCode Basics:** Opening folders and editing files.

## **3\. Introduction: Why NumPy? (Reading)**

While Python lists are flexible, they are slow for data science. Imagine you have 1,000,000 rows of sales data. To multiply every row by a 10% tax in a Python list, Python has to look at every single "box" one by one, check what's inside, and then do the math.

**NumPy (Numerical Python)** changes this. It uses **Vectorization**, which allows it to perform math on the entire "block" of data at once. It is often 10x to 100x faster than standard Python and uses much less memory.

**Key Concept to Watch For:** The `ndarray`. This is the primary object we will use to hold our data. Unlike a Python list, every item in an `ndarray` *must* be the same data type (e.g., all integers or all floats).

**Goal for Class:** Move from "looping through data" to "performing operations on data blocks."
