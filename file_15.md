# 📌 Bitwise Operators in C 🚀

Bitwise operators directly work on binary (0s & 1s) and are used to modify individual bits efficiently. In C, there are 6 types of bitwise operators that perform operations on integer values at the bit level.

---

## 🛠 Types of Bitwise Operators in C

---


### 1️⃣ Bitwise AND `(&)`

**Condition:** Both bits must be 1 for the result to be 1.  
**Use:** To check common bits.

| A | B | A & B |
|---|---|--------|
| 0 | 0 | 0      |
| 0 | 1 | 0      |
| 1 | 0 | 0      |
| 1 | 1 | 1      |

**Example:**  

5 & 3
5 = 0101
3 = 0011
& = 0001 → 1
✅ Final Answer: `5 & 3 = 1`

**Where Used:**
- Permission Systems 🔐
- Networking (subnet masks) 🌐
- Flag Checking 🏳️
- Game Development 🎮

---



### 2️⃣ Bitwise OR `(|)`

**Condition:** If any bit is 1, the result is 1.  
**Use:** To combine/set bits.

| A | B | A \| B |
|---|---|--------|
| 0 | 0 | 0      |
| 0 | 1 | 1      |
| 1 | 0 | 1      |
| 1 | 1 | 1      |

**Example:**  

5 | 3
5 = 0101
3 = 0011
| = 0111 → 7
✅ Final Answer: `5 | 3 = 7`

**Where Used:**
- Setting Flags ⚡
- Combining Permissions 🔑
- Network Masking 🌐
- Graphics (color blending) 🎨

---



### 3️⃣ Bitwise XOR `(^)`

**Condition:** If bits are different, result is 1.  
**Use:** Toggling bits, encryption.

| A | B | A ^ B |
|---|---|--------|
| 0 | 0 | 0      |
| 0 | 1 | 1      |
| 1 | 0 | 1      |
| 1 | 1 | 0      |

**Example:**  

5 ^ 3
5 = 0101
3 = 0011
^ = 0110 → 6
✅ Final Answer: `5 ^ 3 = 6`

**Where Used:**
- Cryptography 🔒
- Error Detection ⚡
- Bit Toggling ⚙️
- Game Logic 🎮

---



### 4️⃣ Bitwise NOT `(~)`

**Condition:** Flips all bits (0 → 1, 1 → 0).  
**Use:** Bit flipping, negative number representation.

**Example:**  

~5
5 = 00000101
~ = 11111010 → -6


➡️ Explanation using 2's Complement:
1. Invert 5 → 00000101 → 11111010  
2. Add 1 → 00000110  
3. Decimal = 6  
4. Apply negative sign = `-6`
✅ Final Answer: `~5 = -6`

**Where Used:**
- Flipping Bits 🔄
- Inverse Masks 🎨
- Negative Number Representation ➖
- Network Calculations 🌐

---



### 5️⃣ Left Shift `(<<)`

**Condition:** Shifts bits to the left and fills rightmost with 0.  
**Use:** Multiply by powers of 2.

**Formula:** `a << n = a × (2^n)`

**Example:**

5 << 1
5 = 00000101
<< = 00001010 → 10
✅ Final Answer: `5 << 1 = 10`

**Where Used:**
- Fast Multiplication ➕
- Pixel Positioning 🎨
- Data Compression 📦
- Signal Processing 📡

---



### 6️⃣ Right Shift `(>>)`  

**Condition:** Shifts bits to the right and fills leftmost with 0 (unsigned).  
**Use:** Divide by powers of 2.

**Formula:** `a >> n = a ÷ (2^n)`

**Example:**

16 >> 2
16 = 00010000

= 00000100 → 4
✅ Final Answer: `16 >> 2 = 4`

**Where Used:**
- Fast Division ➗
- Graphics Scaling 🎨
- Image Processing 🖼️
- Embedded Systems ⚙️

---




## 🔁 Summary Table

| Operator | Symbol | Function                        |
|----------|--------|---------------------------------|
| AND      | &      | Common bits (both 1)            |
| OR       | \|     | Any bit is 1                    |
| XOR      | ^      | Different bits only             |
| NOT      | ~      | Flips all bits                  |
| Left Shift | <<   | Multiply by 2ⁿ                 |
| Right Shift | >>  | Divide by 2ⁿ                   |

---

> ✅ Use bitwise operators for speed, efficiency, and low-level hardware access.


✅ Real-World Examples of Bitwise Operators in C

🔐 1. Permission System (File Access) — Using Bitwise AND (&)
🎮 2. Game Development — Collision Detection Using Bitwise AND (&)
🏳️ 3. Flag Setting/Clearing — Using OR (|), AND (&), XOR (^)
🔁 4. Swapping Two Numbers Without Temp Variable — Using XOR (^)
📦 5. Data Compression / Bit Packing — Using Left & Right Shift (<<, >>)
🌐 6. Subnet Mask Calculation in Networking — Using AND (&)
🔄 7. Fast Multiplication/Division — Using <<, >>