# quantcli

CLI tools for the [quantified self](https://en.wikipedia.org/wiki/Quantified_self) — export your personal data from various services so you (and your LLMs) can analyze it.

Output is Markdown by default — well-suited for piping into LLM context, dropping into notebooks, or rendering as-is. Pass `--format json` (or `--format csv`, where supported) for tools that want structured rows.

Every CLI exposes a `prime` subcommand that prints a one-screen primer aimed at LLM agents calling the CLI as a tool. They all share a [single user-facing contract](https://github.com/quantcli/common/blob/main/CONTRACT.md): same date flags (`--since` / `--until`), same output formats, same `auth status` shape.

## Tools

- [crono-export-cli](https://github.com/quantcli/crono-export-cli) — Cronometer (nutrition logs, daily totals, biometrics, exercises, notes)
- [liftoff-export-cli](https://github.com/quantcli/liftoff-export-cli) — Liftoff (gym workouts with sets/reps/weights, bodyweight history)
- [withings-export-cli](https://github.com/quantcli/withings-export-cli) — Withings (activity, sleep, workouts, body measurements, intraday HR/HRV/SpO2)
- [homebrew-tap](https://github.com/quantcli/homebrew-tap) — Homebrew casks for the CLIs
- [common](https://github.com/quantcli/common) — shared contract every CLI follows

## Install

```sh
brew tap quantcli/tap
brew install <tool-name>
```
