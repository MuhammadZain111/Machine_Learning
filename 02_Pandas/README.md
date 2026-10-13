# Pandas Series: Concepts & Practice

A hands-on Jupyter/Colab notebook that walks through the **Pandas Series** data structure, from creation and indexing to boolean filtering, plotting, and commonly used methods. Examples use small toy data plus real-world datasets (YouTube subscriber counts, Virat Kohli's IPL scores, and a Bollywood movies/actors list).

## What's Inside

| Section | Topics |
|---|---|
| **Intro** | What Pandas is; what a Series is (a 1-D labeled array) |
| **Creating a Series** | From lists, with custom index, with `name`, from dictionaries |
| **Attributes** | `size`, `dtype`, `name`, `is_unique`, `index`, `values` |
| **Reading data** | `pd.read_csv(..., index_col=..., squeeze=True)` to load a one-column CSV as a Series |
| **Inspecting** | `head`, `tail`, `sample`, `value_counts`, `sort_values`, `sort_index` |
| **Math methods** | `count`, `sum`, `mean`, `median`, `mode`, `std`, `var`, `min`, `max`, `describe` |
| **Indexing & slicing** | Integer, negative, slice, fancy (list) and label indexing; assigning values; adding new labels |
| **Python functions on Series** | `len`, `type`, `sorted`, `min`/`max`, `list()`, `dict()`, `in` operator, looping |
| **Operators** | Arithmetic broadcasting, relational operators |
| **Boolean indexing** | Counting 50s/100s and ducks, days with >200 subscribers, actors with >20 movies |
| **Plotting** | Line plot (`subs.plot()`), pie chart of `value_counts()` |
| **Important methods** | `astype`, `between`, `clip`, `drop_duplicates`, `duplicated`, `isnull`, `dropna`, `fillna`, `isin`, `apply`, `copy` |

## Requirements

- Python 3.8+
- `pandas`
- `numpy`
- `matplotlib` (for plotting)

```bash
pip install pandas numpy matplotlib
```

## Datasets

The notebook expects these CSV files (loaded from Colab's `/content/` directory):

| File | Used as | Description |
|---|---|---|
| `subs.csv` | `subs` | Daily YouTube subscriber counts (one column) |
| `kohli_ipl.csv` | `vk` | Virat Kohli's runs per IPL match, indexed by `match_no` |
| Movies/actors CSV | `movies` | Movie title to lead actor mapping (index = movie title) |

> **Note:** the cell that loads `movies` is not included in the notebook. Add a `read_csv` cell for it before running the cells that use `movies`.

## How to Run

**Google Colab**
1. Upload `Pandas.ipynb` to Colab (or open it from Drive).
2. Upload the CSV files to the session storage (`/content/`).
3. Run the cells top to bottom.

**Locally**
```bash
jupyter notebook Pandas.ipynb
```
Update the file paths (e.g. `/content/subs.csv` to `data/subs.csv`) to match your setup.

## Known Issues

- **`squeeze=True` in `read_csv`** was removed in pandas 2.0. On newer versions, use:
  ```python
  subs = pd.read_csv('subs.csv').squeeze('columns')
  vk = pd.read_csv('kohli_ipl.csv', index_col='match_no').squeeze('columns')
  ```
- **Typos in a few cells** (`marks_seriesd`, `subsd`, `copyd`) will raise `NameError`. Remove the trailing `d`.
- **`movies` is undefined** until you load it (see Datasets).
- **Negative indexing on labeled Series** (e.g. `marks_series[-1]`) is deprecated; use `.iloc[-1]`.
- The **"Copy and Views"** section and the final `copy` cell are placeholders with no content yet.

## Learning Outcomes

After working through the notebook you should be able to:
- Create and inspect Series from different Python objects and files
- Select and modify data using positional and label-based indexing
- Filter data with boolean conditions
- Summarize, clean, and transform a Series with built-in methods
- Plot a Series quickly for exploration

## License

Free to use for learning purposes.
