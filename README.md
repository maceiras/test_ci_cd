# Simple FastAPI Example

Super simple FastAPI REST API with one endpoint and one test.

## Structure

```
test_pytest/
├── app/
│   ├── __init__.py
│   └── main.py          # FastAPI app with 1 endpoint
├── tests/
│   ├── __init__.py
│   └── test_main.py     # 1 test
└── pyproject.toml       # All dependencies here
```

## Install & Run

```bash
pip install -e .
uvicorn app.main:app --reload
```

## Test

```bash
pytest
```

## Endpoint

- `GET /` - Returns `{"message": "Hello World"}`