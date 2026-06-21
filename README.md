# skills

[![skills.sh](https://skills.sh/b/jaggedmountain/skills)](https://skills.sh/jaggedmountain/skills)

A collection of [agent skills](https://skills.sh/), one directory per skill.

Install or run with the [`skills`](https://skills.sh/) CLI.

## Skills

### [one-mind](one-mind/SKILL.md)

Speak as one mind with the user — first-person pronouns (`I`, `we`, `us`) or
none, never second person. It applies the voice in-session and offers to install
the rule permanently into your `CLAUDE.md`, so it holds on every turn rather than
only when the skill happens to load.

**Run it once (recommended) — applies the voice and offers to persist it:**

```sh
npx skills use jaggedmountain/skills@one-mind | claude
```

`use` does not install the skill; it pipes the instructions into the agent for a
single session. The lasting effect comes from the install-into-`CLAUDE.md` step
it offers.

**Or install it so it's available to invoke later:**

```sh
npx skills add jaggedmountain/skills            # project scope
npx skills add jaggedmountain/skills -g         # global scope
```

`add` makes the skill available but does not run it; invoke it (e.g. `/one-mind`)
to trigger the persist step.

## License

MIT
