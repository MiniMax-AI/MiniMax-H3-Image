# MiniMax-H3-Image Skills

This directory contains the skills bundled with [MiniMax-H3-Image](../README.md). Each skill lives in its
own folder with an installable `SKILL.md` and the references and scripts it needs.

## Installation

Install skills with the [skills CLI](https://github.com/vercel-labs/skills):

```bash
# List all skills available in this repository
npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --list

# Install a single skill
npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --skill h3-image-prompt-writing
```

## Skills

### h3-image-prompt-writing

<p align="center">
  <img src="../assets/h3-image-prompt-writing.jpg" alt="Three images rendered from prompts the skill wrote: a 3:4 poster titled 雨夜集市 for a night market in the rain, latte art poured into a white cup in a café, and a library on a floating island above the clouds with airships moored beside it" width="560">
</p>

Write MiniMax-H3-Image prompts for text-to-image and editing from an idea, a brief, an existing prompt
or reference images. The prompt describes the whole image in English, keeps literal text in its original
language, names reference images `<Picture 1>`, `<Picture 2>`, ... in order, and comes with an aspect
ratio. The skill follows the official [Prompting Tips](../README.md#prompting-tips) and ships with:

- [`references/t2i-en.txt`](h3-image-prompt-writing/references/t2i-en.txt): text-to-image
- [`references/edit-en.txt`](h3-image-prompt-writing/references/edit-en.txt): editing with reference images
- [`scripts/generate.py`](h3-image-prompt-writing/scripts/generate.py): renders the prompt through the
  MiniMax API, as written for text-to-image (the API always expands editing prompts). It reads the key
  from `MINIMAX_API_KEY`; with a China-platform key, also set `MINIMAX_API_BASE=https://api.minimax.cn`

[SKILL.md](h3-image-prompt-writing/SKILL.md)

## Contribute

The skills are still being improved. If you improve a skill or add a new one, please open a pull
request.
