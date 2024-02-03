---
title: "Linear Algebra: Your Beginner's Guide to Matrices and Transformations."
datePublished: Wed Jan 24 2024 09:04:07 GMT+0000 (Coordinated Universal Time)
cuid: clrrk6eq2000409l63wvmdp4s
slug: linear-algebra-your-beginners-guide-to-matrices-and-transformations
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1706086963921/c93302d1-b36a-4028-ad99-92c9705a9c56.jpeg
tags: machine-learning, beginner, mathematics, linear-algebra

---

A linear equation is simply an equation with no variable whose power is greater than 1. A linear equation is always a polynomial of degree 1.  
Example of linear equation:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706083382817/1a8bcc34-dd5b-4983-81f0-62dea8bdc80b.png align="left")

Example of nonlinear equation:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706083447103/1609cb80-425b-4ee2-b998-3f098507f216.png align="left")

*A system of linear equations is a collection of one or more linear equations*. Example:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706083793281/5379bcb4-10a5-4c59-bc2b-92f34e261bf0.png align="center")

It is possible to solve this system using the elimination or substitution method, but it is also possible to do it with matrix operation. Before we start setting up matrices, it is important to remember that each equation in the system becomes a row, and each variable in the system becomes a column. The variables are dropped and the coefficients are placed into a matrix. If the right-hand side is included it is called an augmented matrix. if the right-hand side is not included, it’s called a coefficient matrix. An example would be better to understand :

Consider a linear system

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706083926526/fd4cacca-5b58-47f1-a4d3-1dd67325ca20.png align="center")

The matrix

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706083966580/7ae6f89d-2a5d-45d5-a09a-4898321e8fce.png align="left")

Is called the <mark>coefficient matrix</mark> of the given linear system and the matrix

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706084276114/dd9d1bbe-eace-44e3-b2c9-d21f33a587ce.png align="left")

is called the <mark>augmented</mark> matrix of the system.

### Furthermore, three types of solutions are possible when solving a system of linear equations.

Every system of linear equations has no solutions, has exactly one solution, or has infinitely many solutions. Systems of equations fall into *two* categories: ***consistent systems and inconsistent systems.*** A system of equations that has **no solution** is said to be **inconsistent**, *which is one in which the equations represent parallel lines.*

**Case-1 (inconsistent):**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706084548581/f9b7da23-5ed2-46e5-b3a7-09c215e9327b.png align="center")

 $$ 2x+3y=6, 4x+6y=5$$

**Case-2 (consistent and one unique solution):**

If there is ***at least one*** solution in the system, it is called **consistent**. A consistent system is considered to be an ***independent*** system if it has a **single solution**, such lines have different slopes and intersect at one particular point.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706084968241/ae232ae2-ae96-49de-bba4-3b00497aee87.png align="center")

**Case-3 (consistent and infinite number of solutions):**

A consistent system is considered to be a ***dependent*** system if the lines coincide <mark>(overlap with each other)</mark> so the equations represent the same line. Every point on the line represents a coordinate that satisfies the system. Thus, there are an **infinite number of solutions.**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706085073744/2c2e0d97-33b2-4225-978d-99d044722915.png align="center")

An arbitrary system of m linear equations in n unknowns can be written as:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706085551013/42a4c3e0-c3d1-4f85-a63f-7bb581883555.png align="center")

where x1, x2.....xn, are the unknowns and the subscripted a's and b's denote constants.