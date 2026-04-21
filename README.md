# Updating The Website

Only edit these files:

- `index.md` = homepage
- `bio.md` = bio page
- `work.md` = work page
- `assets/img/` = images

## Basic rules

- Edit the text directly in the `.md` files.
- Normal links use:
  `[Text](https://example.com)`
- Images used inside the page use:
  `![Alt text]({{ '/assets/img/filename.jpg' | relative_url }})`
  ex. '![Headshot]({{ '/assets/img/headshot.jpeg' | relative_url }})'

## Work page hover images

In `work.md`, if you want a link to show an image on hover, use:

```md
[Project title](https://example.com "preview: {{ '/assets/img/filename.jpg' | relative_url }}")
```

Put the image file inside `assets/img/`.

## Adding a new work item

Example:

```md
1. [Project title](https://example.com "preview: {{ '/assets/img/filename.jpg' | relative_url }}"), short description (2026)
```

If no hover image is needed:

```md
1. [Project title](https://example.com), short description (2026)
```

## Do not edit unless needed

- `_layouts/`
- `assets/style.css`
- `_config.yml`

## Preview locally

Run:

```bash
bundle exec jekyll serve
```

Then open:

`http://127.0.0.1:4000/Basicwebsite/`
