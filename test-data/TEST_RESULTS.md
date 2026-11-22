# Sample Function Test Results

**Scope:** The sample `findMaximum` function shown in the project demonstration. The C++ implementation was compiled with `g++ -std=c++17 -O2`; the Python implementation was run with Python 3. Each non-empty test input was supplied to both implementations and the returned values were compared.

**Result:** 10/10 non-empty test cases produced matching outputs.

| # | Scenario | Input | C++ output | Python output | Result |
|---:|---|---|---:|---:|---|
| 1 | Normal mixed values | [10, 25, 7, 18] | 25 | 25 | PASS |
| 2 | Ascending order | [1, 2, 3, 4, 5] | 5 | 5 | PASS |
| 3 | Reverse order | [9, 7, 5, 3, 1] | 9 | 9 | PASS |
| 4 | All negative | [-8, -3, -12, -1] | -1 | -1 | PASS |
| 5 | Duplicate maximum | [4, 9, 2, 9, 1] | 9 | 9 | PASS |
| 6 | Single element | [42] | 42 | 42 | PASS |
| 7 | Large positive integer | [100000, 2147483647, 999999] | 2147483647 | 2147483647 | PASS |
| 8 | Repeated values | [6, 6, 6, 6] | 6 | 6 | PASS |
| 9 | Zero and negatives | [-5, 0, -2, -1] | 0 | 0 | PASS |
| 10 | Maximum at first position | [99, 2, 30, 4] | 99 | 99 | PASS |

## Edge-case analysis

- **Empty vector/list:** Not included in the cross-language execution comparison. The original C++ implementation reads `numbers[0]`; an empty vector therefore causes undefined behaviour. The Python candidate explicitly raises `ValueError("Input list cannot be empty")`. This is a deliberate safety improvement, not identical behaviour.
- **Single element:** Confirmed matching output.
- **Negative values and duplicates:** Confirmed matching output.
- **Integer boundary:** The tested maximum is the largest signed 32-bit integer. Values outside the C++ `int` range were not tested and are not directly comparable to Python's arbitrary-precision integers.

## Complexity review

- Scan: O(n) time in both implementations.
- Python auxiliary algorithm space: O(1), excluding the input list.
- C++ signature takes `vector<int>` by value, so the argument copy can require O(n) additional storage before the scan. This signature-level cost should not be hidden by describing only the loop.

## Interpretation

These results support matching outputs for the ten listed non-empty inputs for this specific example. They do not establish correctness for arbitrary programs, test the browser interface, evaluate model-generated translations at scale, or provide a formal proof of semantic equivalence.
