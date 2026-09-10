# Pandas Fundamentals Practice

A structured practice series covering core pandas operations, plus two applied feature-extraction projects on real datasets.

## Features
- Series creation from lists, arrays, and dictionaries
- Merging, joining, and concatenating DataFrames (inner/outer/left/right)
- GroupBy and aggregation (single-key, multi-key, multi-function `.agg()`)
- Pivot tables and cross tables
- Core DataFrame operations: shape, info, describe, broadcasting, `.apply()`
- Feature extraction from raw scraped text fields (episode counts, date ranges) on an anime ratings dataset
- Feature extraction and conditional filtering (population extremes, region counts, string matching) on a countries dataset

## Tech Stack
- Python 3.13
- pandas
- numpy
- re (standard library)
- datetime (standard library)

## Dependencies
`pandas`, `numpy`

## Installation
```bash
pip install pandas numpy
```

## Usage
Open any notebook in Jupyter and run cells top to bottom. The two notebooks under `projects/` expect `anime.csv` and `Countries.csv` in the same working directory (see `projects/data/`).

## Notes / Limitations
- `feature_extraction_anime.ipynb` parses episode count and air-date range from a raw scraped `Title` string field; parsing assumes a `(N eps)` pattern is present somewhere in the title.
- Requires the two CSV datasets to be present locally — they are not bundled by pandas itself.
