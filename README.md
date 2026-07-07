# Skills

A skill is a folder with a `SKILL.md` file in it. The front matter (`name` and
`description`) tells Claude what the skill does and when to reach for it; the
body is the instructions Claude follows once the skill fires.

## Skills in this repo

- **[explain-clearly](explain-clearly/SKILL.md)** — Explain technical things in
  plain English: lead with the impact, drop the jargon, spell out why it
  matters.

## Installing a skill

Put the skill's folder in `~/.agents/skills`, then symlink it into
`~/.claude/skills` so Claude discovers it:

```
mkdir -p ~/.agents/skills ~/.claude/skills
cp -R explain-clearly ~/.agents/skills/
ln -s ~/.agents/skills/explain-clearly ~/.claude/skills/explain-clearly
```

The folder name and the `name` in the front matter should match. Claude
discovers the skill on its next run — no restart or registration step needed.

## License

[MIT](LICENSE)
