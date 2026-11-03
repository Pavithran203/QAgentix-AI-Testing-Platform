# QAgentix AI Testing Platform

An AI-assisted software testing platform combining a FastAPI backend and agent framework with a React/Vite frontend and configurable model-provider integrations.

## Example: turn a requirement into a test

A sample requirement might be: **When a shopper enters an expired card, checkout should show a clear validation message and must not place the order.** In a configured QAgentix workspace, use the requirement to draft a test case, review the generated steps, select the configured model provider, and execute the approved browser test. Treat generated cases as drafts that need review before they run against a real service.

## Included
- Backend/app/, Backend/src/, and Backend/tests/: API, agent framework, provider integrations, and tests.
- Frontend/src/ and npm manifests: web client source and build configuration.
- docs/, projects/example/, and config templates: documentation, starter project, and local setup.
- Full source tree: project-source.zip at the repository root. Download and extract it before setup.

Local .env files, generated workspaces, caches, build output, and presentation notes are excluded. Add your own provider keys to a local .env; never commit secrets.

## Setup

Backend requires Python 3.12. In Backend/, create a Python 3.12 virtual environment, install the project dependencies, then run playwright install chromium. Copy the root .env.example to .env and add only provider keys you are authorized to use. In Frontend/, run npm install and npm run dev.

See the included backend and frontend READMEs for project-specific commands and configuration.
