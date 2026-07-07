# Skills

A small collection of [Claude](https://claude.com) skills by true-and-useful.

A skill is a folder with a `SKILL.md` file in it. The front matter (`name` and
`description`) tells Claude what the skill does and when to reach for it; the
body is the instructions Claude follows once the skill fires.

## Skills in this repo

- **[explain-clearly](explain-clearly/SKILL.md)** — Explain technical things in
  plain English: lead with the impact, drop the jargon, spell out why it
  matters.

## Installing a skill

Copy the skill's folder into one of the places Claude looks for skills.

**Claude Code — for one project** (only that project sees it):

```
mkdir -p .claude/skills
cp -R explain-clearly .claude/skills/
```

**Claude Code — for every project** (available everywhere on your machine):

```
mkdir -p ~/.claude/skills
cp -R explain-clearly ~/.claude/skills/
```

The folder name and the `name` in the front matter should match. Claude
discovers the skill on its next run — no restart or registration step needed.

## License

[MIT](LICENSE)
