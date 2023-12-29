# MatrixLib

This project a Java library for matrix operations, supporting parallel and sequential matrix implementations. The library includes basic matrix operations such as addition, subtraction, dot product, Hadamard product, cloning, equality checking, and printing matrices.

## MatrixLib Overview

The library consists of the following key components:

- **matrix**: An abstract class providing a foundation for both sequential and parallel matrix implementations. It includes common matrix operations as abstract methods.

- **matrixFactory**: A factory class for creating instances of the matrix. It includes methods for creating sequential or parallel matrices with specific dimensions or from a given 2D array.

- **sequentialMatrix**: A concrete implementation of the matrix with sequential computation for basic operations.

- **parallelMatrix**: A concrete implementation of the matrix with parallel computation for enhanced performance.

- **main**: The main class provides a command-line interface for users to interact with the matrixLib functionalities. It prompts users to input matrix dimensions, select matrix operations (addition, subtraction, multiplication, or Hadamard product), and displays the result.

## Getting Started

### Prerequisites

- Java Development Kit (JDK)

### Usage

1. Clone the repository.

   ```bash
   git clone git@github.com:MSO03/matrix-operations.git
   ```

2. Open the project in your preferred Java development environment.

3. Run the `main` class to interact with the library through a command-line interface.

4. Utilize the MatrixLib classes based on your requirements.

## Example

```java
// Creating sequential matrices
Matrix A = MatrixFactory.getSequentialMatrix(3, 3);
Matrix B = MatrixFactory.getSequentialMatrix(new double[][]{{1, 2, 3}, {4, 5, 6}, {7, 8, 9}});

// Performing matrix addition
Matrix result = A.add(B);

// Printing the result
System.out.println(result.toString());
```