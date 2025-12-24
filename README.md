# data-engineering-zooomcamp
Data Engineer zoomcamp

## Pipeline usage ✅

Run the ingestion script from the `pipeline` folder. Example commands:

- Using `uv` (recommended if you use `uv` to manage the virtual environment):

  ```bash
  uv run python ./pipeline/ingest_data.py --year 2021 --month 1 --pg-user root --pg-pass root --pg-host localhost --pg-port 5432 --pg-db ny_taxi --chunksize 100000 --target-table yellow_taxi_data
  ```

- Directly with Python (if `click` is installed in your environment):

  ```bash
  python pipeline/ingest_data.py --help
  ```
