# Functions

## 1. Definition of a Function

A function is defined as a **TRIPLE OF OBJECTS** (Domain, Codomain, Rule).

A function is a correspondence f: A → B such that:
* **A** is the starting set, called the **Domain**.
* **B** is the arrival set, called the **Codomain**.
* **The Rule (f)** establishes the correspondence between elements.

### Fundamental Rule (Property of Correspondences)
* **Every element of A** must be put into correspondence.
* **Every element of A** is put into correspondence with **one and only one element of B**.

![Interval](media/functions/function_def.png)

In this image, functions are marked in green letters, while non-functions are marked in red:  
- Image **A** is not a function because not all elements of the first set are put into correspondence.  
- Image **B** is not a function because the third element of the first set is put into correspondence with multiple elements of the second set.  
- Image **C** is a function because all elements of the first set have exactly one correspondence with elements of the second set.  
- Image **D** is a function since there is no rule stating that all elements of the second set must have a correspondence.  

### Graph of a Function
The **Graph of f** (graph(f)) is a subset of the **Cartesian Product** A × B.  
graph(f) = {(a, b) in A × B : b = f(a)}

Example: Taking as the Cartesian product A × B the relation ℝ × ℝ (i.e., the Cartesian plane itself), the pair (a, b) of points belongs to the graph only if it satisfies the function f, meaning b = f(a).    
Practical Example: f(x) = x²   
The function f(x) = x² (Domain ℝ, Codomain ℝ) works as follows:    
f(2) = 4  
f(-1) = 1  
f(0) = 0  

The graph of f is the set of these points:
graph(f) = {..., (-1, 1), (0, 0), (2, 4), ...}

### Image of a Function

* **Image of D subset of A**: The set f(D) = {f(x) : x in D}.
    * **In simple terms**: It is the set of all output values (y) that the function produces when we consider **ONLY a subset (D)** of the domain.

    * **Example**: If f(x) = x² (Domain ℝ) and we consider the subset D = [1, 2] (only numbers between 1 and 2).
        * f(D) = [1, 4]. (The image is the set of all numbers between 1² = 1 and 2² = 4).

* **Image of the Function (Im(f))**: The image of the entire domain, Im(f) = f(A).
    * **In simple terms**: It is the set of **all output values (y)** that the function can reach in absolute terms. It is the projection of the graph onto the y-axis.

    * **Example**: If f(x) = x² (Domain A = ℝ, Codomain B = ℝ).
        * Im(f) = [0, +∞). (The function can never produce negative numbers but starts from 0 and goes to infinity).

* **Key Relationship**: Im(f) is always a subset of the Codomain (B).
    * Im(f) and B are equal **only if** the function is surjective.

---

## 2. Properties of Functions

### A. Injectivity
* **Definition**: A function f: A → B is called **injective** if distinct elements of the domain correspond to distinct elements in the codomain.
    * If x₁ ≠ x₂, then f(x₁) ≠ f(x₂).

* **Graphical Criterion**: Every horizontal line intersects the graph at **at most one point**.

![injective](media/functions/injective.png)  
The function on the left is injective because by drawing horizontal lines we will never find two points of contact with the graph, while the function on the right is not injective because horizontal lines can be found that touch the graph twice.  

### B. Surjectivity
* **Definition**: A function f: A → B is called **surjective** if the image of the function coincides with the entire codomain.
    * For every y in B, there exists AT LEAST ONE x in A such that f(x) = y.
    * **Im(f) = B**.

* **Graphical Criterion**: Every horizontal line drawn in the codomain intersects the graph at **at least one point**.  
![surjective](media/functions/surjective.png)  
The function on the left is surjective because by drawing horizontal lines we will always find at least one point of contact with the graph, while the function on the right is not surjective because horizontal lines can be found that never touch the graph.  

### C. Bijectivity (Invertible)
* **Definition**: A function is **bijective** if it is **BOTH injective and surjective**.

* **Graphical Criterion**: Every horizontal line intersects the graph at **EXACTLY ONE point**.  
![bijective](media/functions/bijective.png)  
The function on the left is bijective because by drawing horizontal lines we will always find exactly one point of contact with the graph, while the function on the right is not bijective because it can be seen that the red horizontal lines touch the graph more than once. 

## 3. Inverse Function (f⁻¹)

### Fundamental Requirement: Bijectivity
* **Rule**: Only **bijective** functions admit an inverse function, denoted by f⁻¹.

### Definition and Transformation
* The inverse function exchanges the roles of domain and codomain: f⁻¹: B → A.
* **Formal Definition**:
f⁻¹(b) = a ⟺ f(a) = b
    * **In simple terms**: The inverse takes a value b (output of f) and returns its original input a.

### Rationale: Why is Bijectivity Needed?
* **Rationale**: The function must be both injective and surjective to ensure that for every element b in B, there exists **one and only one** element a in A that corresponds to it (i.e., such that f(a) = b).

1.  **Surjectivity Guarantees Existence**:
    * **Explanation**: For every b in B (the new Domain), surjectivity ensures that *there exists at least* one element a in A such that f(a) = b. There are no "gaps" in the original Codomain.

2.  **Injectivity Guarantees Uniqueness**:
    * **Explanation**: Injectivity ensures that the element a found is **unique**. Without this property, the inverse would not know which of two (or more) values of a to return.

* **Conclusion**: Only when it is bijective can the inverse function be defined uniquely, as we are certain it will maintain the characteristics seen in the "Fundamental Rule (Property of Correspondences)" previously discussed.

![inverse](media/functions/inverse.png)