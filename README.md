# bigint

## Big Integer Library for C++

### 1 Million digits? 1 Billion? 1 Trillion? No worries. This library can handle any integer of any length.

`bigint` is a C++ library that can handle very large __Big Integers__. It can calculate the *factorial* of numbers like __1000000__ and beyond. It's ideal for use in *competitive coding*, *scientific calculations*, and *decryption processes*. With numerous built-in functions, it offers flexibility and simplicity when working with huge numbers.

---

```c++
#include "bigint.h"     // with proper file path 
Declaring and Initializing Variables
Declaration is done like creating an object of the bigint class.
Initialization supports string, int, or long types.

c++
Copy
Edit
bigint a("56654250564056135415631554531554513813");     // string initialization
bigint b("60820564691661355463515465564664568");
bigint d(956486133);                                    // integer initialization
Arithmetic Operations
➕ Addition
c++
Copy
Edit
bigint c = a + b;
cout << c << std::endl;

c = a + 56242;
c = 52 + 98;
c = c + a + b;
➖ Subtraction
c++
Copy
Edit
c = a - b;
c = a - 56242;
c = 52 - 98;
c = c - a - b;
✖️ Multiplication
c++
Copy
Edit
c = a * b;
c = a * 56242;
c = 52 * 98;
c = c * a * b;
➗ Division
c++
Copy
Edit
c = a / b;
c = a / 56242;
c = 98 / 56;
c = a / b / c;
% Modulo
c++
Copy
Edit
c = a % b;
c = a % 56242;
c = 98 % 56;
c = a % b % c;
🧠 Conditional Statements
Supports:

>, <, >=, <=, ==, !=

c++
Copy
Edit
if (a > b) {
    cout << "a is greater than b" << std::endl;
}

if (a != b) {
    cout << "a is not equal to b" << std::endl;
}
⚙️ In-built Functions
to_bigint(...) – Converts from string / int / long to bigint
c++
Copy
Edit
b = to_bigint("56");
big_abs(bigint) – Absolute value
c++
Copy
Edit
b = to_bigint("-60820564691661355463515465564664568");
cout << big_abs(b) << std::endl;
big_max(a, b) – Maximum of two bigints
big_min(a, b) – Minimum of two bigints
big_pow(a, b) – Power
big_sqrt(a) – Square root (floor value)
big_log2(a) – Log base 2 (floor value)
big_log10(a) – Log base 10 (floor value)
big_logwithbase(a, b) – Log base b of a (floor value)
c++
Copy
Edit
cout << big_logwithbase(a, b) << std::endl;
big_swap(a, b) – Swaps two bigint variables
c++
Copy
Edit
big_swap(a, b);
big_gcd(a, b) – Greatest Common Divisor
big_lcm(a, b) – Lowest Common Multiple
big_fact(a) – Factorial
big_isPrime(a) – Prime check (true / false)
big_reverse(a) – Digit reversal
big_isPalindrome(a) – Palindrome check (true / false)
⬆️ Increment and ⬇️ Decrement
c++
Copy
Edit
++a;
--a;
📦 Installation
Just include bigint.h in your C++ project. No dependencies required.

✅ Requirements
C++11 or later

Works with all major compilers

✨ Author
Sarthak Singh