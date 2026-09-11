# PySpark Data Processing

A collection of notebooks exploring PySpark RDD and DataFrame operations, file formats, and batch analysis using Titanic passenger data.

## Notebooks

| Notebook | Contents |
|---|---|
| [01_spark_api.ipynb](01_spark_api.ipynb) | RDD transformations and actions, partitioning, DataFrame filtering, aggregation, and joins |
| [02_file_formats.ipynb](02_file_formats.ipynb) | Reading CSV and JSON data, writing and reading Parquet files |
| [03_batch_processing.ipynb](03_batch_processing.ipynb) | Passenger counts, age statistics, and survival rates by passenger characteristics |

## Project Structure

```text
pyspark-data-processing/
├── 01_spark_api.ipynb
├── 02_file_formats.ipynb
├── 03_batch_processing.ipynb
└── data/
    ├── titanic.csv
    └── titanic.json
```

## Running the Notebooks

Use a notebook environment with PySpark and a compatible Java runtime. The first notebook uses `Column.try_cast`, which requires PySpark 4.0 or later.

1. Download or clone this repository.
2. Open the notebooks with the repository root as the working directory.
3. Keep the datasets inside the `data/` folder.
4. Run each notebook from top to bottom.

For Google Colab, upload the notebook and create a `data/` folder containing the datasets before running it.

The notebooks generate a local `titanic_parquet/` folder. This output is recreated when the relevant write cells run.

## Analysis Notes

The batch analysis includes passenger counts and survival rates by class, sex, embarkation port, and cabin information.

Age analysis uses two different groupings: consecutive age
