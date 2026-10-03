# EZ Statements ZM website: implementation guide

A static landing and download website explaining the EZ Statements ZM mobile utility.

## Scope

**Repository role:** Project landing page.

Download binaries and claims need to match the current app release. The website itself does not retrieve or authenticate examination results.

## Local evaluation

Run a static server from the repository root:

```sh
python -m http.server 4173
```

Open `http://localhost:4173` and select the relevant HTML page or variant directory. No build step is required for plain HTML/CSS/JavaScript. Use a server when scripts fetch local content; opening a file directly can produce different behavior.

## Code map

| Path | Responsibility |
| --- | --- |
| `index.html` | Page or browser application entry |
| `script.js` | Browser interaction behavior |
| `style.css` | Presentation and responsive styles |

## Walkthrough

Read the app explanation, follow the download/help route, and verify that the linked release exists and has an accurate version label.

## Verification

No meaningful automated application check was established from the reviewed manifest. Evaluate the walkthrough with synthetic data and record the commit, environment, and result. For a static site, inspect narrow/wide layouts, keyboard focus, links, forms, and console errors.

## Evidence for a case study

Describe this repository as a **project landing page**. A useful case study explains the problem above, traces the walkthrough to its source, names a concrete implementation decision, and records a repeatable evaluation. Separate implemented behavior from roadmap work. Capture screenshots using synthetic data and identify the demonstrated commit.
