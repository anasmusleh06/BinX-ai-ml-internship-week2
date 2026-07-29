# Day 3 — Linear Algebra for ML:

## Overview
This lab covers the linear-algebra objects every ML model runs on: vectors, matrices, the dot product and matrix multiplication. It applies them directly to a mini "predict a score for each customer" scenario.

## What's inside

 1. Vectors & Matrices | Represents 3 customers (`age, income, tenure`) as a `(3, 3)` NumPy matrix 
 2. Dot Product | Computes one customer's weighted score by hand, then verifies with `np.dot` 
 3. Matrix Multiplication | Uses `X @ weights` to predict a score for all 3 customers in a single operation 
 4. Shape Mismatch | Deliberately triggers a `ValueError` with a mismatched weight vector, then explains the cause and the fix 

## Key takeaway

A linear model's prediction is just: `prediction = dot(features, weights) + bias`. Matrix multiplication scales that single operation across an entire dataset at once — and shape mismatches (inner dimensions not matching) are the most common bug in ML code.
