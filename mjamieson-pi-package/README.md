# Personal Pi Package

This package is the safe place for your own `pi` customizations in this repo.

## Why This Exists

- Keeps personal `pi` changes out of upstream-tracked files.
- Makes upstream pulls and rebases much less likely to conflict.
- Travels with the repo because `.pi/settings.json` loads it with a relative path.

## Put Customizations Here

- `extensions/` for `.ts` or `.js` extensions
- `skills/` for skill folders containing `SKILL.md`
- `prompts/` for reusable `.md` prompt templates
- `themes/` for custom `.json` themes

## Recommended Workflow

1. Leave upstream `pi` code alone when possible.
2. Put your personal behavior changes in this package.
3. Commit these files in your own branch or fork.
4. Pull or rebase upstream changes as usual.

## Another Computer

1. Clone your repo on the other computer.
2. Run `npm install` in the repo if needed.
3. Start `pi` from this repo and it will load this package automatically.

If you want to publish or separately version your customizations later, you can move this directory into its own repo or npm package without changing the structure.
