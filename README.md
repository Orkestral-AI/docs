<div align="center">

<img src="logo/dark.svg" width="72" alt="Orkestral" />

# Orkestral Documentation

Official documentation for **Orkestral**, the local-first desktop app where a team of AI agents plans, executes and reviews your code.

**Live:** [docs.orkestral.pro](https://docs.orkestral.pro) · **Product:** [orkestral.pro](https://orkestral.pro)

</div>

---

## About

This is the [Mintlify](https://mintlify.com) project that powers `docs.orkestral.pro`. It is **bilingual** (English + Brazilian Portuguese) and documents the Orkestral desktop app: getting started, the agent team, the Forge, day-to-day work, power features, how-to guides and a reference section.

## Structure

```
docs/
├─ docs.json        Navigation, theme, languages (en + pt)
├─ style.css        Custom CSS (scrollbar)
├─ logo/            Orkestral logos (light + dark)
├─ en/              English pages (.mdx)
└─ pt/              Portuguese pages (.mdx)
```

Navigation is split into **Get started**, **Learn** (Day to day, Your org & agents, Projects & workflow, Power features, How-to guides, Administration) and **Reference** (Adapters, MCP server, Integrations).

## Writing conventions

- **Bilingual:** every page exists in both `en/` and `pt/` with the same slug. When you add or change a page, update both languages.
- **No em-dashes:** never use the `—` / `–` characters. Use commas, parentheses or colons.
- **Accurate to the app:** document the real behavior of the desktop app (the code lives in the `orkestral` repo). Do not invent features.
- **Components:** use Mintlify components (`Steps`, `Tabs`, `Accordion`, `Card`, `Note`, `Tip`, `Warning`) to stay visual and instructive.
- **Screenshots:** `{/* PRINT: ... */}` markers indicate where a screenshot of the app should go.

## Develop locally

Install the Mintlify CLI and run the dev server from this folder (where `docs.json` is):

```bash
npm i -g mint
mint dev
```

Preview at `http://localhost:3000`, with the EN/PT switcher in the top bar.

## Publishing

Changes pushed to the default branch (`main`) are deployed automatically to `docs.orkestral.pro` by the Mintlify GitHub app. No manual build step.

---

<div align="center">

Built for the [Orkestral](https://orkestral.pro) desktop app.

</div>
