# QAgentix AI Testing Platform

> Full source tree is included in `project-source.zip` at the repository root. Unpack it to restore the directories and files summarized below.

QAgentix is an AI-assisted software testing platform for designing, generating, executing, and reporting tests. It combines a FastAPI backend and agent framework with a React/Vite frontend and configurable model-provider integrations.

## Included files

- `Backend/app/`, `Backend/src/`, and `Backend/tests/`: API, agent framework, provider integrations, and tests.
- `Frontend/src/` and frontend npm manifests: web client source and build configuration.
- `docs/`, `projects/example/`, and config templates: documentation, starter project, and local setup.

Local `.env` files, generated workspaces, caches, build output, and presentation notes are excluded. Add your own provider keys to a local `.env`; never commit secrets.

## Setup

Backend requires Python 3.12. Unpack the source archive, then from `Backend/` run `py -3.12 -m venv .venv`, activate it, `pip install -e ".[dev]"`, and `pip install -r requirements.txt`. Install the Playwright browser with `playwright install chromium`. Copy the root `.env.example` to `.env` and add only your own provider keys.

For the frontend, run `npm install` and `npm run dev` from `Frontend/`.
