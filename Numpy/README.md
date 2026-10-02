# NumPy Arrays: Concepts & Practice

A beginner-friendly Jupyter/Colab notebook that covers the fundamentals of **NumPy**: creating arrays, generating data, indexing and slicing, arithmetic and broadcasting, copying, matrix operations, and stacking/splitting.

## What's Inside

| Section | Topics |
|---|---|
| **Creating arrays** | `np.array` from lists, mixed types (upcast to strings), nested lists to 2-D arrays |
| **Generation functions** | `arange`, `zeros`, `linspace`, `random.rand`, `random.randn`, `random.randint` |
| **Attributes & methods** | `shape`, `size`, `sum`, `min`, `max`, `mean`, `std`, `np.sum(arr, axis=...)` |
| **Reshaping** | `reshape` (e.g. 30 elements to 6x5) |
| **Indexing & slicing** | 1-D indexing, `start:stop:step` slices, 2-D slicing (rows, columns, sub-matrices) |
| **Boolean indexing** | Filtering with conditions such as `arr % 2 == 0` |
| **Arithmetic** | Element-wise `+`, `-`, `*`, `/` |
| **Broadcasting** | Adding a scalar to 1-D and 2-D arrays |
| **Copying** | Reference vs. `.copy()` behavior |
| **Matrix operations** | Element-wise `*` vs. `np.dot`, transpose with `.T` |
| **Array manipulation** | `vstack`, `hstack`, `column_stack`, `hsplit` |

## Requirements

- Python 3.8+
- `numpy`

```bash
pip install numpy
```

## How to Run

**Google Colab**
1. Upload `Numpy.ipynb` to Colab or open it from Drive.
2. Run the cells top to bottom (no external datasets needed).

**Locally**
```bash
jupyter notebook Numpy.ipynb
```

## Key Takeaways

- Lists with mixed types become **string arrays** (`<U32`) when converted with `np.array`.
- `shape` and `size` are **attributes** (no parentheses); `sum()`, `min()`, `max()` are **methods**.
- In 2-D arrays, indexing is `arr[row, column]`; `arr[:, 2]` selects a whole column.
- Boolean masks filter arrays: `arr[arr % 2 == 0]`.
- Broadcasting applies scalars across every element: `arr + 10`.
- `A * B` is **element-wise**; true matrix multiplication needs `np.dot(A, B)` or `A @ B`.

## Known Issues & Corrections

Some cells will raise errors or contain notes that are slightly off:

- **`np.random.randint(10, 2)`** raises `ValueError` because low must be less than high. Use `np.random.randint(2, 10)`.
- **`np.dot(A, B)`** fails with the shapes used (both are 2x3). Use `np.dot(A, B.T)` or define a matrix with 3 rows for `B`.
- **Transpose note:** `A.T` works on any 2-D array. The matrices don't need to be square.
- **Copy terminology is swapped.** `b = a` creates a reference (both names point to the same array), and `a.copy()` creates an independent copy (a deep copy). Slices like `a[:5]` are *views* that share memory with the original.
- **`arr.min()` note** in the markdown describes it as a sum; it returns the minimum.
- **`np.linspace(1, 5, 2)`** returns only the two endpoints `[1., 5.]`; it doesn't give "2 elements between 1 and 5".
- Some cells (e.g. `np.sum(arr, axis=0)`, `column_stack((a, b))`) depend on variables defined earlier; run the notebook in order.

## Learning Outcomes

After working through the notebook you should be able to:
- Create arrays from lists and with generator functions
- Inspect and reshape arrays
- Select data with indexing, slicing, and boolean masks
- Apply arithmetic and broadcasting operations
- Understand views vs. copies
- Perform basic matrix operations and combine or split arrays

## License

Free to use for learning purposes.
