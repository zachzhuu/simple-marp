# Simple Marp - My Customized Marp Theme

This repository contains a customized [Marp](https://marp.app/) theme, forked from the excellent Marp Academic Theme. This allows you to create your presentation slides with `Markdown` and `HTML`.

## Usage

Best viewed with [CMU fonts](https://ctan.org/pkg/cm?lang=en).

Add the following code to the VSCode user `setting.json`:

```json
"markdown.marp.themes": [
    "./themes/academic.css"
]
```

Then use this theme with your [Marp](https://marp.app/) slides by importing it in your Markdown front-matter:

```markdown
---
marp: true
theme: academic
---
```

There is a sample in `page.md`.

## Acknowledgments
Original theme by [Marp](https://marp.app/) and [kaisugi](https://github.com/kaisugi/marp-theme-academic).
