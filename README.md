# oboard/numoon

## 📖Table of Contents

- [Introduction](#-introduction)
- [Getting Started](#-getting-started)
- [Contributing](#-contributing)
- [License](#-license)

## ✨Introduction

**Numoon** is an open-source MoonBit library that provides support for multi-dimensional array objects and functions for efficiently operating on these arrays.

<!-- The core of Numoon is its N-dimensional array object NMArray, which is very similar to basic MoonBit lists but can store any data type and perform vectorized mathematical operations. This makes Numoon highly suitable for numerical computations. -->

Here are some key features of Numoon:

1. Multi-dimensional Array Objects: Numoon provides a powerful N-dimensional array NMArray, which is the foundation for scientific computing.

2. Derived Objects (such as Masked Arrays and Matrices): Numoon allows users to create special arrays, like masked arrays, which handle missing or invalid data.

3. Extensive Mathematical Function Library: Numoon has a vast array of mathematical functions, including linear algebra, Fourier transforms, and random number generation.
<!-- 
4. Vectorized Operations: Numoon's array operations are vectorized, meaning you can perform operations on arrays without explicit loops.

5. Support for Various Data Types: Numoon supports a wide range of data types, including integers, floating-point numbers, complex numbers, and more.

6. Operation Broadcasting: Numoon offers a powerful mechanism that allows arithmetic operations between arrays of different sizes.

7. Memory Efficiency: Numoon arrays store data more efficiently than native MoonBit data structures.

8. Tool Integration: Numoon is the foundation for many other scientific computing libraries, such as SciMoon, Moondas, and MoonPlotlib. -->

Numoon is an indispensable tool for scientific computing and data analysis in MoonBit, widely used in fields such as physics, biology, engineering, and more.

## 🚀Getting Started

To get started with Numoon, you can simply install it using the following command:

```bash
moon install oboard/numoon
```

This will install the latest version of Numoon and its dependencies.

To use Numoon in your MoonBit program, simply import the library using the following code:

You can then create an NMArray object using the following code:


### Creating Arrays

```moonbit
a = @nm.int_array([1, 2, 3])
b = @nm.int_array([1, 2, 3])
printLn(a + b) 
// Output: [2, 4, 6]
```

This creates a 1-dimensional array of integers and performs vectorized addition.

```moonbit
a = @nm.double_array([1.0, 2.0, 3.0])
```

### Random Number Generation

```moonbit
let list1 = @nm.rand(2, 3)
println(list1)
// Output: [[0.2893123275883688, 0.33959090191249325, 0.1521095035725017],
//  [0.9314055834969763, 0.8561914513327412, 0.7919828439328577]]
```

### Matrix

```moonbit
let list1 = @nm.int_matrix([[1, 2, 3], [4, 5, 6]])
```

#### Matrix Operations
```moonbit
let m2 = @nm.int_matrix([[1, 2, 3], [4, 5, 6]])
let m1 = @nm.int_matrix([[7, 8], [9, 10], [11, 12]])

let result = @nm.dot(m1, m2)
println(result)

// Output: [[121.0 136.0 151.0]
//  [153.0 172.0 191.0]
//  [185.0 208.0 231.0]]
```
#### Matrix Transpose
```moonbit
let a = @nm.int_matrix([[1, 2], [3, 4]])

println(a.transpose())

// Output: [[1 3]
//  [2 4]]
```


## 🤝Contributing

We welcome contributions to Numoon! Please read our [contribution guide](CONTRIBUTING.md) to learn more.

## 👨‍💻Authors
- @oboard
- @Yorkin

## 📝License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
