# Pelican

Example [Pelican](https://getpelican.com/) static site. Pelican is a Python static site generator that builds sites from Markdown or reStructuredText.

## Deploy settings

| Field | Value |
| --- | --- |
| Build | Static site — Railpack build |
| Single-page application (SPA) | off |
| Project directory | `/` |
| Output directory | `/output` |
| Install command | leave empty |
| Build command | `pelican content` |
| Health check path | `/` |

## <a name="dev"></a>Run locally

```bash
# virtual environment and dependencies
python3 -m venv .venv
. .venv/bin/activate
pip install -r requirements.txt

# run in development mode
pelican --autoreload --listen

# build for production
pelican content
```

Requires Python 3.10 or later.
