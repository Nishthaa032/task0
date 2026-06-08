# MLOps Technical Assessment

## Local Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Run:

```bash
python run.py \
  --input data.csv \
  --config config.yaml \
  --output metrics.json \
  --log-file run.log
```

## Docker

Build:

```bash
docker build -t mlops-task .
```

Run:

```bash
docker run --rm mlops-task
```

## Example Output

```json
{
  "version": "v1",
  "rows_processed": 10000,
  "metric": "signal_rate",
  "value": 0.4990,
  "latency_ms": 127,
  "seed": 42,
  "status": "success"
}
<img width="985" height="235" alt="image" src="https://github.com/user-attachments/assets/c97e2d77-6017-48c8-b95d-63528c4727aa" />

```
