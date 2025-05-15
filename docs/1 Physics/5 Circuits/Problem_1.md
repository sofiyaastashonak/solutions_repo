# Problem 1

# ⚡ Circuits Problem 1  
## Equivalent Resistance Using Graph Theory  

---

## ✅ 1. Motivation  

Calculating equivalent resistance is a key task in circuit analysis. Traditionally, this involves applying **series and parallel rules**, but for **complex resistor networks**, these manual methods become inefficient and error-prone.

Graph theory provides a powerful alternative. By modeling the circuit as a **weighted graph**:

- Nodes represent junctions,
- Edges represent resistors (weights = resistance),
- The task becomes a problem of graph simplification.

This method allows for **algorithmic**, repeatable, and programmable solutions — which are especially useful in circuit simulation software.

---

## ✅ 2. Problem Setup  

We consider a circuit modeled as a graph with:

- Nodes representing **junctions**,
- Edges representing **resistors** (with resistance values as weights),
- One **START** node and one **END** node.

The goal is to find the **equivalent resistance** between START and END by simplifying the graph using algorithmic steps based on electrical principles.

---

## ✅ 3. Theoretical Concepts  

### 🔹 Ohm’s Law  
$$V = IR$$

### 🔹 Series Resistance  
If resistors $R_1$ and $R_2$ are in **series**: 

$$R_{\text{eq}} = R_1 + R_2$$

### 🔹 Parallel Resistance  
If resistors $R_1$ and $R_2$ are in **parallel**: 

$$\frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2}$$

---

## ✅ 4. Graph-Based Strategy  

We represent the circuit as a **graph**:
- Vertices = junctions
- Edges = resistors with weights
- Start and end nodes are marked

The simplification proceeds by:
- Identifying nodes with **degree = 2** (series),
- Identifying **multiple edges** between the same nodes (parallel),
- Iteratively applying reduction rules until a single edge remains.

---

## ✅ 5. Algorithm Overview  

**Step-by-step simplification algorithm:**

1. Find nodes with degree 2 (excluding START and END).
2. Apply **series rule** to combine two adjacent resistors.
3. Find **multiple edges** between two nodes.
4. Apply **parallel rule** to combine them.
5. Repeat steps until only one edge connects START to END.

---

## ✅ 6. Example: Complex Circuit

We use the following network:

- Resistors between: START–A, A–B, B–C, C–END
- Also additional edges: A–C and B–END

This graph includes both series and parallel combinations.

![alt text](image.png) 
(Shows all nodes and resistors with weights)

![alt text](image-1.png)  
(Combines those resistors)

![alt text](image-2.png)
(Combines A–C paths in parallel with earlier A–C edge)

![alt text](image-3.png) 
(This edge shows the final equivalent resistance)

[Colablink](https://colab.research.google.com/drive/1Gnqf6nJ7SUzUnyfO8ePysKOdNfTIPay3?usp=sharing)
---

## ✅ 7. Results and Output  

After simplification, the graph is reduced to a single edge between **START** and **END**. The final equivalent resistance is computed and returned.

🧮 **Final Equivalent Resistance**:  
**Approximately**: 

$$R_{\text{eq}} \approx 4.36\ \Omega$$

---

## ✅ 8. Analysis and Efficiency  

- Graph reduction steps are efficient and can be automated.
- Works for any **nested** configuration of resistors.
- Algorithm scales well for larger, complex networks.
- Complexity: approximately 
$$\mathcal{O}(n \log n)$$ 
with efficient detection of patterns.

---

## ✅ 9. Conclusion  

This graph-based method of simplifying resistor networks:

- Provides a **structured and scalable** solution,
- Can be implemented in code for use in **circuit simulators**,
- Highlights the deep connection between **physics** and **graph theory**.

It is especially valuable in modern contexts such as:
- PCB design tools,
- Educational simulators,
- Automated testing and optimization.

📌 This approach can be extended to capacitors, AC impedance networks, or even mesh current/loop analysis for complex AC circuits.

---


