# Finite Automata Project – Discrete Mathematics (LU2IN005)

This project implements a complete set of algorithms for **finite automata** using Python.  
It was developed as part of the *Mathématiques Discrètes – LU2IN005* course at **Sorbonne Université (2023-2024)**.

The notebook and Python files provided by the instructors define base data structures.  
All algorithmic implementations and functions inside `automate_etudiant.ipynb` were coded by the students.

---

## Project Overview

This project builds a full toolkit to manipulate **finite automata**, including:

- Representing **states**, **transitions**, and **automata** using OOP in Python  
- Constructing automata from:
  - sets of transitions
  - sets of states
  - external description files
- Implementing classical automata algorithms:
  - successor computation (`succElem`, `succ`)
  - acceptance of words
  - determinism and completeness checks
  - completion of non-complete automata
  - determinization

It also includes advanced constructions from automata theory:

- **Complement**
- **Intersection**
- **Union**
- **Concatenation**
- **Kleene star** (étoile)

All functions were extensively tested with multiple examples.

---

## Project Structure

- automate_etudiant.ipynb # Main notebook with all implementations
- state.py # Provided class representing states
- transition.py # Provided class representing transitions
- automateBase.py # Base class for Automate
- ExemplesAutomates/ # Example automata files
- affichage.dot # Graphviz display file (if generated)


The **only file modified by the students** is:

- `automate_etudiant.ipynb`

---

## Implemented Functions

### Basic Tools
- `succElem` — successor from one state
- `succ` — successor from a *set* of states
- `accepte(mot)` — checks if a word is accepted
- `estComplet(Alphabet)` — completeness check
- `estDeterministe()` — determinism check

### Automata Transformations
- `completeAutomate(Alphabet)`
- `newLabel(S)` — canonical label for determinization
- `determinisation()`

### Language Operations
- `complementaire(Alphabet)`
- `intersection(auto2)`
- `union(auto2)`
- `concatenation(auto2)`
- `etoile()`

Each function is accompanied by multiple test cases.

---

## Concepts Covered

This project demonstrates strong understanding of:

- Formal languages & automata theory  
- Deterministic / nondeterministic finite automata  
- Python OOP and structured programming  
- Graph exploration & transition systems  
- Language operations (∪, ∩, ⋅, *)  
- Determinization algorithms  
- Automata completion and complement  

