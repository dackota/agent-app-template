# agent-app-template

PROTOTYPE. Start here to put an agent on the platform.

1. Click "Use this template".
2. Put your code in `app.py` (or replace it). Read `LLM_BASE_URL`, `LLM_API_KEY`,
   `LLM_MODEL`, and, if you asked for tools, `TOOLS_URL` and `TOOLS_TOKEN`.
   Never add your own model keys.
3. Fill in `agent.yaml`. Bump `VERSION` and the image tag together.
4. Push to `main`. The shared workflow builds, signs, and publishes your image.
5. Open a PR that adds your `agent.yaml` to the platform repo. The platform deploys it.

Your app must answer `GET /healthz` with 200.
