# Clinic Management System (Custom 2-3 Tree Implementation)

## Overview
This project is a high-performance Java application designed to manage a medical clinic's doctors and their patient waiting rooms. To ensure optimal execution times, the system is built entirely on a custom, from-scratch implementation of a **2-3 Search Tree**.

## Technical Highlights
*   **Custom Data Structures:** Implements a balanced 2-3 Search Tree to handle insertions, deletions, and lookups without relying on standard Java collections libraries.
*   **Augmented Trees:** Features an augmented `LoadTree` that maintains subtree sums to allow for advanced range queries (e.g., finding the average patient load across specific doctors).
*   **Strict Time Complexities:** Designed to meet strict algorithmic constraints, ensuring core operations run in logarithmic time:
    *   Adding/Removing Doctors: `O(log D)`
    *   Adding/Removing Patients: `O(log D + log P)`
    *   Statistical Range Queries: `O(log D)`

## Core Components
*   `ClinicManager.java`: The primary controller routing all clinic operations.
*   `TwoThreeTree.java`: The foundational balanced search tree logic.
*   `LoadTree.java`: An extended 2-3 tree utilizing augmented node data to calculate statistics across given ranges in logarithmic time.
*   `Doctor.java` & `Patient.java`: Object models managing state and individual, nested waitlist trees.

## Testing
The `tests/` directory contains rigorous simulation logs verifying system stability and algorithmic correctness under high load and complex edge cases.
