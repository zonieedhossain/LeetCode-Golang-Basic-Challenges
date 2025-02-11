# 📌 LeetCode Golang Basic Challenges

**Practice essential Golang concepts with curated LeetCode problems.**

This repository provides a structured way to improve your **loops, conditionals, string manipulation, slices, recursion, and algorithm logic** using Go. Each problem has its own directory where contributors can add their optimized solutions.

---

## **Folder Structure**
```
basic-loops-conditionals/
│   ├── fizz-buzz/
│   ├── count-primes/
│   ├── power-of-three/
│   ├── divisor-game/
│   ├── number-of-steps-to-zero/
string-manipulation/
│   ├── reverse-string/
│   ├── reverse-words-in-string-iii/
│   ├── valid-palindrome/
│   ├── longest-common-prefix/
│   ├── first-unique-character/
working-with-slices/
│   ├── maximum-subarray/
│   ├── find-peak-element/
│   ├── third-maximum-number/
│   ├── kth-largest-element/
│   ├── find-disappeared-numbers/
algorithm-logic/
│   ├── valid-palindrome/
│   ├── palindrome-number/
│   ├── longest-palindromic-substring/
│   ├── palindrome-linked-list/
│   ├── palindrome-partitioning/
recursion/
│   ├── factorial-trailing-zeroes/
│   ├── climbing-stairs/
│   ├── fibonacci-number/
│   ├── pow-x-n/
│   ├── generate-parentheses/
sum-even-numbers/
│   ├── sum-even-numbers-queries/
│   ├── two-sum/
│   ├── count-odd-numbers/
│   ├── add-digits/
│   ├── subtract-product-sum/
CONTRIBUTING.md
README.md
```

---

## **How to Contribute**
1. **Fork this repository** and **clone your fork**
```bash
git clone https://github.com/your-username/LeetCode-Golang-Basic-Challenges.git
```
2. **Create a new branch** for your contribution:
```bash
git checkout -b feature/new-solution
```
3. **Navigate to the correct problem folder** and **add your solution**
```bash
cd basic-loops-conditionals/fizz-buzz
```
4. **Write your optimized solution (`solution.go`)**
```go
// Optimized Fizz Buzz Solution (Beats 95%+ runtime)
package main

import "strconv"

func fizzBuzz(n int) []string {
  result := make([]string, n)
  for i := 1; i <= n; i++ {
    switch {
    case i%15 == 0:
      result[i-1] = "FizzBuzz"
    case i%3 == 0:
      result[i-1] = "Fizz"
    case i%5 == 0:
      result[i-1] = "Buzz"
    default:
      result[i-1] = strconv.Itoa(i)
    }
  }
  return result
}
```
5. **Write a test file (`solution_test.go`)** to verify correctness:
```go
package main

import "testing"

func TestFizzBuzz(t *testing.T) {
  expected := []string{"1", "2", "Fizz", "4", "Buzz", "Fizz", "7", "8", "Fizz", "Buzz"}
  result := fizzBuzz(10)
  for i, v := range result {
    if v != expected[i] {
      t.Errorf("Expected %v but got %v at index %d", expected[i], v, i)
    }
  }
}
```
6. **Run tests to verify your solution:**
```bash
go test -v ./...
```
7. **Commit and push your changes:**
```bash
git add .
git commit -m "Added optimized solution for Fizz Buzz (LeetCode #412) - Beats 95%+ runtime"
git push origin feature/new-solution
```
8. **Create a Pull Request** on GitHub and include:
- **A brief description of your solution**
- **LeetCode runtime performance screenshot** (if possible)
- **Ensure the code follows Go best practices**

---

## **Contribution Guidelines**
✅ **Well-optimized solution** (runtime beats at least **90%**).
✅ **Proper function naming & inline comments**.
✅ **Include a test case** in a separate `*_test.go` file.
✅ **Follow Go best practices** (error handling, variable naming, etc.).
✅ **Attach LeetCode runtime screenshot** (if possible) in the PR description.

---

### **📌 Summary**
- `README.md` → **Overview**, **folder structure**, and **usage instructions**.
- `CONTRIBUTING.md` → **How to contribute**, **coding standards**, and **submission process**.

This will keep your project **well-organized** and **easy for contributors to understand**. Let me know if you need any modifications!



