# Base44 Dev Environment

## Project
Simple Streamlit app (`streamlit_app.py`) with a single dependency: `streamlit` (see `requirements.txt`).

## Running
- `docker compose -f docker-compose.base44.yml up -d --build`
- App is served on host port **3000** (Streamlit internal port 3000).
- Streamlit auto-reloads on file changes (live source served, no build step).

## Health Check
- Streamlit health endpoint: `http://localhost:3000/_stcore/health`

## Notes
- No external services or secrets required.
- XSRF protection is disabled for the dev preview; CORS is enabled.
