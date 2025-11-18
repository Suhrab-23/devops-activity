# C8. DevOps Activity
Suhrab Roeen 100811513

## Implemented Features
- **Endpoints:**
  - `GET /` (default route)
  - `POST /echo`: Accepts JSON payload and echoes it back with status 201.
- **Tests:**
  - Automated test for `/echo` endpoint in `test_app.py` to verify correct response and status code.

- **CI/CD Workflows:**
  - Automated testing and CodeQL security scanning configured in `.github/workflows/`.

## Issues Encountered
- **CodeQL Action Warning:**
  - Received warnings about deprecated `@v1` version. Fixed by updating to `@v2` in the workflow file.
- **Matrix Build Failure:**
  - Python version error (`3.1` not found). Resolved by quoting Python versions in the matrix: `["3.10", "3.11", "3.12"]`.

## How to Run
- All endpoints and tests are covered by CI using GitHub Actions.
- Push changes to trigger tests and security scans automatically.
