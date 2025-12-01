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

- automate_etudiant.ipynb
Main project notebook.
Contains all student-implemented functions: acceptance, determinization, completion, intersection, union, concatenation, étoile, etc.

- automateBase.py: 
Base class provided by the instructors.
Implements the core structure of an Automate (states, transitions, base methods).
Students do not modify this file.

- state.py: 
Defines the State class (ID, initial flag, final flag, label).
Used to create and manipulate states in an automaton.

- transition.py: 
Defines the Transition class (source state, label, destination state).
Used to build transition systems.

- myparser.py: 
A helper script (provided).
Used to parse automata description files or text structures into Python objects.

- sp.py: 
Small supporting Python script (provided).
Usually contains utility functions or helper operations used internally by the base automaton classes.

- affichage.dot: 
GraphViz DOT file generated when calling automate.show().
Represents the structure of an automaton as a graph.

- affichage.dot.png: 
PNG image automatically generated from affichage.dot.
Visual rendering of the automaton graph.


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

