# Construction PM Hub

A lightweight, single-file project management app for construction PMs — built for Hillsdale Flats and the DC Bio-Retention project.

## Features

- **Dashboard** — high-priority tasks, project progress, upcoming events
- **Tasks** — add, complete, and delete tasks with priority and due dates
- **RFIs** — log and track RFIs with status, assignee, and due dates
- **Submittals** — track submittals by spec section, sub, return due date, and approval status
- **Calendar** — visual monthly calendar with meetings and deadlines
- **Contacts** — contact cards for subs, reviewers, and engineers
- **Generate** — Claude AI-powered content generator for emails, agendas, minutes, and more

## Hosting on GitHub Pages

1. Create a new GitHub repository (e.g. `construction-pm`)
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch` → `main` → `/ (root)`
5. Click **Save**
6. Your app will be live at `https://YOUR-USERNAME.github.io/construction-pm`

## Using the AI Generator

The Generate tab uses the Anthropic API. To use it:

1. Get an API key at [console.anthropic.com](https://console.anthropic.com)
2. Open the Generate tab in the app
3. Paste your key into the API key field and click **Save key**
4. Your key is stored in your browser's localStorage — it never leaves your device

## Data Storage

All project data (tasks, RFIs, submittals, contacts, events) is saved in your browser's localStorage. Data is per-device and persists between sessions.

## Customizing

The entire app is a single `index.html` file. Open it in any text editor to:
- Change project names in the `DEF` object at the top of the script
- Add or edit prompt templates in the `PROMPTS` object
- Adjust colors in the `:root` CSS block
