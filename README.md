# Quick Bites Kitchen

Daily recipe site powered by AI. New recipe added every day.

**Live site**: https://kitchen.neatbites.com

## What it is

- 60+ recipes and growing
- Recipes generated daily by Ollama (qwen3:8b)
- Categories: quick-meals, air-fryer, desserts, soups, bowls, pasta, breakfast, healthy
- Deployed via GitHub Pages

## How it works

1. Daily cron runs `scrapers/kitchen-content/run.sh`
2. Ollama generates a unique recipe as JSON
3. Recipe is saved as HTML and committed to this repo (`gh-pages` branch)
4. GitHub Pages deploys automatically to kitchen.neatbites.com

## Tech stack

- AI: Ollama + qwen3:8b
- Hosting: GitHub Pages
- Analytics: Cloudflare Web Analytics
- Automation: Bash + cron
