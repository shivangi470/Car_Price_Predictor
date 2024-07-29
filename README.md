# BigInt-Library-

Overview

The BigInt library is a C++ library designed to handle large integers that exceed the standard data type limits (int, long long). This library supports a wide range of operations such as arithmetic operations, comparisons, and various mathematical functions, making it a powerful tool for applications requiring high-precision calculations.
Features

    Arithmetic Operations: Addition, subtraction, multiplication, division, and modulus.
    Increment and Decrement: Pre-increment, post-increment, pre-decrement, and post-decrement.
    Comparison Operators: Equality, inequality, less than, greater than, less than or equal to, and greater than or equal to.
    Utility Functions: Factorial, nth Fibonacci, and nth Catalan numbers.
    Input/Output: Stream operators for easy input and output.
    Mathematical Functions: Power and square root functions.

Class Methods
Constructors

    BigInt(unsigned long long n = 0): Initializes a BigInt from an unsigned long long integer.
    BigInt(const string &s): Initializes a BigInt from a string representing a large number.
    BigInt(const char *s): Initializes a BigInt from a C-string.
    BigInt(const BigInt &a): Copy constructor.

Helper Functions

    friend void divideBy2(BigInt &a): Divides the BigInt by 2.
    friend bool isNull(const BigInt &a): Checks if the BigInt is zero.
    friend int length(const BigInt &a): Returns the number of digits in the BigInt.
    int operator[](const int index) const: Accesses the digit at the given index.

Operator Overloading

    Assignment, increment, and decrement operators:
        BigInt &operator=(const BigInt &a)
        BigInt &operator++()
        BigInt operator++(int)
        BigInt &operator--()
        BigInt operator--(int)

    Arithmetic operators:
        friend BigInt &operator+=(BigInt &a, const BigInt &b)
        friend BigInt operator+(const BigInt &a, const BigInt &b)
        friend BigInt operator-(const BigInt &a, const BigInt &b)
        friend BigInt &operator-=(BigInt &a, const BigInt &b)
        friend BigInt &operator*=(BigInt &a, const BigInt &b)
        friend BigInt operator*(const BigInt &a, const BigInt &b)
        friend BigInt &operator/=(BigInt &a, const BigInt &b)
        friend BigInt operator/(const BigInt &a, const BigInt &b)
        friend BigInt operator%(const BigInt &a, const BigInt &b)
        friend BigInt &operator%=(BigInt &a, const BigInt &b)
        friend BigInt &operator^=(BigInt &a, const BigInt &b)
        friend BigInt operator^(const BigInt &a, const BigInt &b)

    Comparison operators:
        friend bool operator==(const BigInt &a, const BigInt &b)
        friend bool operator!=(const BigInt &a, const BigInt &b)
        friend bool operator<(const BigInt &a, const BigInt &b)
        friend bool operator>(const BigInt &a, const BigInt &b)
        friend bool operator<=(const BigInt &a, const BigInt &b)
        friend bool operator>=(const BigInt &a, const BigInt &b)

Special Functions

    friend BigInt nthCatalan(int n): Returns the nth Catalan number.
    friend BigInt nthFibonacci(int n): Returns the nth Fibonacci number.
    friend BigInt factorial(int n): Returns the factorial of n.

I/O Operations

    friend ostream &operator<<(ostream &out, const BigInt &a): Outputs the BigInt.
    friend istream &operator>>(istream &in, BigInt &a): Inputs a BigInt

This documentation provides an overview of the BigInt library, its features, and its usage. The library can be extended with more features and optimized further based on specific requirements.
