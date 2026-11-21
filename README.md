# AI-Team-26 · Landing Page

Landing page for the [AI-Team-26](https://github.com/AI-Team-26) organization. It lists the public repositories, grouped by type, with a short note per project.

## How it works

The page is plain HTML, CSS and JavaScript, with no build step.

- `index.html` holds the repository list.
- `style.css` holds the styles.

The list is written by hand. This keeps the page simple and lets us add custom text, notes and images per project, instead of showing raw data from the GitHub API.

## Add or edit a repository

1. Open `index.html`.
2. Find the section that fits the repository: *AI & Agents*, *Editor & Browser Extensions*, or *Apps & Services*.
3. Copy an existing `<article class="card">` block and change the title, link, description and note.
4. Add a note like `C# · small tools` in `<p class="card-note">` when it helps.

### Add an image to a card

1. Put the file in an `images/` folder, for example `images/ai.models-evaluator.png`.
2. Uncomment the image line inside the card:

```html
<img class="card-image" src="images/ai.models-evaluator.png" alt="">
```

## Preview locally

Open `index.html` in a browser, or run a small local server:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Publish on GitHub Pages

Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.

The expected URL is <https://ai-team-26.github.io/github-page/>.

> **Note:** this repository is private. GitHub Pages from a private repository needs GitHub Pro or a paid organization plan. On the free plan the repository must be public.

## Repository layout

```
index.html    repository list
style.css     styles
TODO.md       task list
```