# BigInt – C++ Big Integer Library

A lightweight, header-only C++ library for working with **arbitrarily large integers**, with intuitive syntax and full support for arithmetic, relational operations, and utility functions — all without external dependencies.

---

## 📦 Features

- Supports integers far beyond `long long` range
- Simple `+`, `-`, `*`, `/`, `%` operations using operator overloading
- Relational operators: `==`, `!=`, `<`, `<=`, `>`, `>=`
- Utility functions: GCD, power, factorial, etc.
- Single-header library – easy to include and use
- Well-documented and beginner-friendly

---

## 📁 File Structure

BigINT/
│
bigint.h # Single-header Big Integer library ---
SampleTest.cpp # Sample test file with usage examples ---
bigint_function_definitions.h # Function bodies (if modularized) ---
bigint class.h # Class definition (if modularized) ---
.vscode/settings.json # Optional: VS Code settings


---

## 🚀 Getting Started

### 1. **Include the Header**

Copy `bigint.h` to your project and include it:

```cpp
#include "bigint.h"
2. Example Usage
cpp
Copy
Edit
#include <iostream>
#include "bigint.h"

int main() {
    BigInt a = "123456789123456789123456789";
    BigInt b = "987654321987654321987654321";

    BigInt sum = a + b;
    BigInt diff = b - a;
    BigInt prod = a * b;
    BigInt quot = b / a;
    BigInt rem = b % a;

    std::cout << "Sum: " << sum << "\n";
    std::cout << "Difference: " << diff << "\n";
    std::cout << "Product: " << prod << "\n";
    std::cout << "Quotient: " << quot << "\n";
    std::cout << "Remainder: " << rem << "\n";

    return 0;
}
✅ Supported Operations
Operation	Syntax	Example
Addition	a + b	BigInt c = a + b;
Subtraction	a - b	BigInt c = a - b;
Multiplication	a * b	BigInt c = a * b;
Division	a / b	BigInt c = a / b;
Modulo	a % b	BigInt c = a % b;
Comparisons	==, !=, <, >	if (a > b) {}
Assignment	=, +=, -=, *=	a *= 10;

🛠 Advanced Functions (Optional)
If implemented:

gcd(a, b) – returns greatest common divisor

power(a, n) – returns a^n

factorial(n) – returns n!

📚 Sample Test
Refer to SampleTest.cpp in this repo for more usage examples and edge case testing.

⚙️ Requirements
C++11 or later

No external dependencies

✍️ Author
Developed by Sarthak Singh

