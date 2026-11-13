# Mission 5: Numbers and Data

## 1. Task / Objective

The objective of this mission was to understand number systems and data representation. I practised converting decimal, binary and hexadecimal numbers manually, verified the conversions using Python, developed a number converter program and explored character encoding using ASCII and UTF-8.

## 2. Work Completed

### Task 5.1: Manual Number System Conversions

I performed the following conversions manually and showed the calculation steps.

**1. Decimal 13 to Binary**

Repeated division by 2:

- 13 ÷ 2 = 6, remainder 1
- 6 ÷ 2 = 3, remainder 0
- 3 ÷ 2 = 1, remainder 1
- 1 ÷ 2 = 0, remainder 1

Reading the remainders from bottom to top:

**(13)₁₀ = (1101)₂**

**2. Decimal 25 to Binary**

- 25 ÷ 2 = 12, remainder 1
- 12 ÷ 2 = 6, remainder 0
- 6 ÷ 2 = 3, remainder 0
- 3 ÷ 2 = 1, remainder 1
- 1 ÷ 2 = 0, remainder 1

Reading the remainders from bottom to top:

**(25)₁₀ = (11001)₂**

**3. Binary 1010 to Decimal**

Using positional weights:

= 1 × 2³ + 0 × 2² + 1 × 2¹ + 0 × 2⁰

= 8 + 0 + 2 + 0

**(1010)₂ = (10)₁₀**

**4. Binary 1101 to Decimal**

= 1 × 2³ + 1 × 2² + 0 × 2¹ + 1 × 2⁰

= 8 + 4 + 0 + 1

**(1101)₂ = (13)₁₀**

**5. Hexadecimal A to Decimal**

In hexadecimal, A represents 10.

**(A)₁₆ = (10)₁₀**

**6. Hexadecimal 1F to Decimal**

In hexadecimal, F represents 15.

= 1 × 16¹ + 15 × 16⁰

= 16 + 15

**(1F)₁₆ = (31)₁₀**

**7. Binary 1111 to Hexadecimal**

Group the four binary digits together:

1111₂ = 15₁₀

The decimal value 15 corresponds to F in hexadecimal.

**(1111)₂ = (F)₁₆**

### Task 5.2: Verification Using Python

I used Python's built-in conversion functions to verify the manual calculations.

| Conversion | Python expression | Result |
|---|---|---|
| Decimal to binary | `bin(13)` | `0b1101` |
| Decimal to binary | `bin(25)` | `0b11001` |
| Binary to decimal | `int('1010', 2)` | `10` |
| Binary to decimal | `int('1101', 2)` | `13` |
| Decimal to hexadecimal | `hex(13)` | `0xd` |
| Decimal to hexadecimal | `hex(25)` | `0x19` |
| Hexadecimal to decimal | `int('A', 16)` | `10` |
| Hexadecimal to decimal | `int('1F', 16)` | `31` |

All the Python conversion results matched the corresponding manual calculations.

### Task 5.3: Building a Number Converter

I created a Python program named `number_converter.py` inside the `mission-05-numbers-data` folder.

The program accepts a positive decimal number from the user and displays its binary and hexadecimal representations.

**Program code:**

```python
# Digital Detective - Mission 5
# Decimal to Binary and Hexadecimal Converter

number = int(input("Enter a positive decimal number: "))

binary_value = bin(number)
hexadecimal_value = hex(number)

print("Decimal:", number)
print("Binary:", binary_value)
print("Hexadecimal:", hexadecimal_value)
```

**Functions used:**

- `input()` accepts the number entered by the user.
- `int()` converts the input string into an integer.
- `bin()` converts an integer into its binary representation.
- `hex()` converts an integer into its hexadecimal representation.
- `print()` displays the results.

**Execution command:**

```bash
python3 number_converter.py
```

**Test results:**

| Decimal input | Binary output | Hexadecimal output |
|---:|---|---|
| 1101 | `0b10001001101` | `0x44d` |
| 12 | `0b1100` | `0xc` |
| 25 | `0b11001` | `0x19` |

I tested the program with three different positive numbers. All three executions produced the correct binary and hexadecimal values.

### Task 5.4: How Is Text Stored?

Computers store text using character encoding standards. These standards map characters to numerical values so that computers can store, process and exchange text consistently.

**ASCII values verified using Python:**

| Character | Python expression | Decimal value |
|---|---|---:|
| Uppercase A | `ord('A')` | 65 |
| Lowercase a | `ord('a')` | 97 |

I also explored a character outside basic ASCII:

- Character: ₹
- Unicode code point: 8377
- UTF-8 encoding: `b'\xe2\x82\xb9'`

**ASCII vs UTF-8:**

- ASCII represents a basic set of 128 characters, including English letters, digits and common symbols.
- UTF-8 is a Unicode encoding that supports characters from many languages, special symbols and emojis.

An encoding standard is necessary because computers store information as binary data. It provides a common mapping between characters and numerical representations, allowing different systems to interpret text correctly.

## 3. Commands / Tools Used

- `cd` – Navigate to the mission directory.
- `code .` – Open the current folder in Visual Studio Code.
- `python3` – Start the Python interactive interpreter.
- `python3 number_converter.py` – Execute the converter program.
- `bin()` – Convert decimal integers to binary strings.
- `hex()` – Convert decimal integers to hexadecimal strings.
- `int(value, base)` – Convert a string from a specified base to a decimal integer.
- `input()` – Accept user input.
- `print()` – Display output.
- `ord()` – Return the Unicode code point of a character.
- `encode('utf-8')` – Encode text using UTF-8.

## 4. My Understanding

Through this mission, I understood how decimal, binary and hexadecimal number systems represent values differently.

I learned how to perform manual conversions and verify them using Python's built-in functions. I also understood how a simple Python program can accept input, process it and display multiple representations of the same number.

I learned that computers need character encoding standards such as ASCII and UTF-8 to represent text as numerical data.

## 5. Difficulties Faced

Initially, I entered some Python expressions directly into the macOS Terminal instead of opening the Python interactive interpreter. This caused a shell error.

I also encountered the Python continuation prompt while entering multiple expressions together, which made the output confusing.

## 6. How I Resolved Them

I started the Python interpreter using `python3` and executed each expression separately at the `>>>` prompt.

I also checked the conversion results against my manual calculations and corrected my understanding of the binary and hexadecimal representations.

## 7. Evidence / Files

The following files are part of this mission:

- `mission-05-numbers-data/README.md` – Mission documentation and calculations.
- `mission-05-numbers-data/number_converter.py` – Python number conversion program.

The Python program was executed successfully with three different positive inputs.

## 8. Commit Details

**Commit message:** `Build number converter and practise data representation`

The mission documentation and Python converter program were committed and pushed to the GitHub repository after completion.