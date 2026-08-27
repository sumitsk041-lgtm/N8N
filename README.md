# Content Engine n8n — Render Ready

1. Push this folder to GitHub.
2. Render → New → Blueprint → connect the repository.
3. Render creates the n8n service and PostgreSQL database from render.yaml.
4. Open the generated n8n Render URL.
5. Set N8N_EDITOR_BASE_URL and WEBHOOK_URL to that exact URL and redeploy.
6. Import content-engine-google-places-discovery.json.
7. Configure Google Places credentials and activate the workflow.
8. Production webhook:
   https://YOUR-N8N-SERVICE.onrender.com/webhook/content-engine/discovery

Existing Scraper_Backend:
Set N8N_WEBHOOK_URL to the production webhook above, then redeploy the backend.

Never commit real API keys or .env files.
