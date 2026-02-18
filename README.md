# Quadratic Polynomial Prediction Dataset

## Project Overview
This dataset contains quadratic polynomials and their roots. The goal is to **predict polynomial characteristics or evaluate polynomial behavior** from given coefficients and roots. This dataset can be used in **machine learning, numerical analysis, or educational experiments**.

---

## Dataset Description
Each row corresponds to a quadratic polynomial of the form:

$$
f(x) = ax^2 + bx + c
$$

**Columns:**

| Column    | Description                                      |
|-----------|--------------------------------------------------|
| `a`       | Coefficient of \(x^2\)                           |
| `b`       | Coefficient of \(x\)                             |
| `c`       | Constant term                                    |
| `x_real_part`  | Real part of the root(s) (if any)               |
| `x_imag_part`  | Imaginary part of the root(s) (0 if root is real)|

> Note: For real roots, `x_imag_part = 0`. For complex roots, `x_real_part` and `x_imag_part` represent the complex number as \(x = x_{\text{real_part}} + i \cdot x_{\text{imag_part}}\).

---

## Dataset Usage
The dataset can be used for:  
- Predicting the roots of a quadratic polynomial from coefficients  
- Training models to classify polynomials with real vs. complex roots  
- Regression tasks to predict coefficients from roots 
- Educational visualization of polynomial behavior

---

## Data Generation / Source
- Coefficients (`a`, `b`, `c`) are generated randomly within a specified range  
- Roots are calculated using the quadratic formula:

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

- Complex roots are represented with separate real and imaginary columns

---

## File Format
- CSV with headers: `a, b, c, x_real_part, x_imag_part`  
- Numeric values (float)

---

## Potential Applications
- ML regression to predict roots from polynomial coefficients  
- ML classification for polynomials with real vs. complex roots  
- Visualization of how coefficients affect polynomial roots  
- Educational tools for algebra and polynomial studies

---

