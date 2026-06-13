# API Contract

## Health Check

### `GET /health`

Used to verify that the external FastAPI service is running.

Example response:

```json
{
  "status": "ok"
}