# MiniMax-H3-Image Skills

This directory contains the skills bundled with [MiniMax-H3-Image](../README.md). Each skill lives
in its own folder with an installable `SKILL.md` and the references and scripts it needs.

## Installation

Install skills with the [skills CLI](https://github.com/vercel-labs/skills):

```bash
# List all skills available in this repository
npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --list

# Install a single skill
npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --skill h3-image-prompt-writing
```

You can also copy a skill folder into your agent's skills directory by hand.

## Skills

### h3-image-prompt-writing

[SKILL.md](h3-image-prompt-writing/SKILL.md)

Turn an idea, a brief, an existing prompt or a set of reference images into a ready-to-use
MiniMax-H3-Image prompt. The skill writes a detailed English description of the whole image,
quoting literal text in its original language and naming reference images `<Picture 1>`,
`<Picture 2>`, ... in the order supplied, and gives an aspect ratio. With `MINIMAX_API_KEY` set, it
renders the prompt when you ask for an image; with a China-platform key, also set
`MINIMAX_API_BASE=https://api.minimax.cn`. It follows the official
[Prompting Tips](../README.md#prompting-tips) and ships with:

- [`references/t2i-en.txt`](h3-image-prompt-writing/references/t2i-en.txt): text-to-image, from
  composition and physical readability to designed artifacts such as posters, charts and UI.
- [`references/edit-en.txt`](h3-image-prompt-writing/references/edit-en.txt): editing with one or
  more reference images, written as source definitions, then the target and what each source keeps
  or lends, then the changed content.
- [`scripts/generate.py`](h3-image-prompt-writing/scripts/generate.py): sends a prompt to the
  MiniMax API for text-to-image or editing and saves the images. It uses only the Python standard
  library and reads the key from `MINIMAX_API_KEY`.

After installing, ask your agent in plain words, for example:

```text
Use h3-image-prompt-writing to make a 3:4 poster of a night market in the rain,
titled "雨夜集市", and render it.
```

For text-to-image, the script sets `disable_prompt_enhanced: true` and passes the aspect ratio, so
the MiniMax API renders the prompt as written; editing requests are always expanded by the API. To
render on your own deployment instead, send the prompt as `prompt` with a `size` from
[Sizes](../README.md#sizes); see [Full Workflow](../README.md#full-workflow).

## Contribute

The skills are still being improved. If you improve the existing skill or add a new one, please
open a pull request.
