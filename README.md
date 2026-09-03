# Software Developer Tactics

A living list of practical rules I want close at hand while building software.

## Data

- Keep data in a database or version-controlled text.
- `.env`-style secrets are an acceptable exception for personal, solo, and open projects, but not at work.
- Microsoft putting secrets in a file that is not named `.env` does not make it a different pattern.

## Git

- Commit `.gitignore` changes immediately, regardless of the current branch. It is not elegant, but accidentally committing ignored files is worse.

## Security and bus factor

- Two-factor authentication apps and their reset procedures all suck. Keep a spare phone with authentication set up in case the main phone is lost or bricked.
  - Some authentication apps sign out inactive devices. Test the spare every three months.

## Windows

- Use one consistent PowerShell version and document its pitfalls.
- Install `ripgrep.exe`.
- Do not burn another afternoon trying to make `rsync` work on Windows.
- When the local Windows setup fights back, move the development environment to a Linux server and connect over SSH.

## Web development

- Web development is mostly solved. If a large part of an application feels unusually hard, I am probably missing a tool, pattern, or piece of information.
- To clean up a CSS codebase buried under `!important`, first inventory every view at each supported resolution and capture screenshots. Use them as visual regression tests while removing the overrides.
