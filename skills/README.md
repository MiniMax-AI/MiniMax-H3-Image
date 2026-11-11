# MiniMax-H3-Image Skills

This directory contains the skills bundled with [MiniMax-H3-Image](../README.md). Each skill lives
in its own folder with an installable `SKILL.md` and the reference material it needs.

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
MiniMax-H3-Image prompt: one detailed English description of the whole image, with literal text
quoted and reference images named `<Picture 1>`, `<Picture 2>`, ... in their supplied order. When
a size is needed, the skill gives the aspect ratio separately; pick the matching size from
[Sizes](../README.md#sizes). It writes prompts only and does not generate images. It ships with
two guides under [`references/`](h3-image-prompt-writing/references/):

- [`t2i-en.txt`](h3-image-prompt-writing/references/t2i-en.txt): text-to-image, from composition
  and physical readability to designed artifacts such as posters, charts and UI.
- [`edit-en.txt`](h3-image-prompt-writing/references/edit-en.txt): editing with one or more
  reference images, written as source definitions, then the target and what each source keeps or
  lends, then the changed content.

After installing, ask your agent for a prompt in plain words, for example:

```text
Use h3-image-prompt-writing to write a prompt for a 3:4 poster of a night market in the rain,
with the title "雨夜集市" at the top.
```

Send the result as `prompt` to your own deployment; see
[Full Workflow](../README.md#full-workflow). With the MiniMax text-to-image API, also set
`disable_prompt_enhanced: true` and the `aspect_ratio` the skill gives, otherwise the API expands
the prompt again; image editing requests are always expanded.

## Contribute

The skills are still being improved. If you improve the existing skill or add a new one, please
open a pull request.
