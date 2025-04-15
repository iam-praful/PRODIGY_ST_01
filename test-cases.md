# 🧪 Calculator Application – Test Cases

This document contains a sample of the test cases designed for the Calculator App (Task 1) as part of the Software Testing Internship at **Prodigy InfoTech**.

---

## ✅ Functional Test Cases

| Test Case ID | Test Description | Preconditions | Test Steps | Expected Result |
|--------------|------------------|---------------|------------|-----------------|
| TC_ADD_01 | Add two positive integers | Calculator is on | Input: `5 + 3 =` | Result: `8` |
| TC_SUB_01 | Subtract a smaller number from a larger number | Calculator is on | Input: `9 - 4 =` | Result: `5` |
| TC_MUL_01 | Multiply two negative numbers | Calculator is on | Input: `-3 * -2 =` | Result: `6` |
| TC_DIV_01 | Divide two positive integers | Calculator is on | Input: `8 / 4 =` | Result: `2` |
| TC_BOD_01 | Test BODMAS: mix of + and * | Calculator is on | Input: `2 + 3 * 4 =` | Result: `14` (if order of operations supported) |

---

## ❌ Invalid Input Test Cases

| Test Case ID | Test Description | Preconditions | Test Steps | Expected Result |
|--------------|------------------|---------------|------------|-----------------|
| TC_INV_01 | Input alphabetic characters | Calculator is on | Input: `A + B =` | Show error / Do not accept input |
| TC_INV_02 | Division by zero | Calculator is on | Input: `9 / 0 =` | Show error or `Infinity` |
| TC_INV_03 | Multiple decimals in one number | Calculator is on | Input: `7..2 + 1 =` | Show error or reject input |
| TC_INV_04 | Click equal without full expression | Calculator is on | Input: `9 +` then `=` | Show error or do nothing |
| TC_INV_05 | Use of special characters | Calculator is on | Input: `9 + # =` | Show error or reject |

---

## ⚠️ Edge Cases

| Test Case ID | Test Description | Preconditions | Test Steps | Expected Result |
|--------------|------------------|---------------|------------|-----------------|
| TC_EDG_01 | Very large number addition | Calculator is on | Input: `999999999 + 1 =` | Result: `1000000000` or scientific notation |
| TC_EDG_02 | Long decimal precision | Calculator is on | Input: `1 / 3 =` | Result: `0.333...` |
| TC_EDG_03 | Multiple sequential operations | Calculator is on | Input: `5 + 2 * 3 - 1 =` | Result depends on operator precedence |
| TC_EDG_04 | Rapid key presses | Calculator is on | Input keys very fast | App does not crash or freeze |
| TC_EDG_05 | Clear button test | Calculator has a value | Press `C` or `AC` | Input should be reset to `0` |

---

### 📝 Notes:
- These are **representative samples**. The full sheet contains 45 test cases categorized into addition, subtraction, multiplication, division, invalid inputs, edge cases, and UI behavior.
- Tests were written and managed using **Excel** for documentation clarity and traceability.

---

🔗 [View Full Test Case Sheet (Excel)](link-to-your-excel-file-on-github)

#ProdigyInfoTech #SoftwareTesting #ManualTesting #CalculatorApp
