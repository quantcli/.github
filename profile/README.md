# quantcli

CLI tools for the [quantified self](https://en.wikipedia.org/wiki/Quantified_self) — export your personal data from various services so you (and your LLMs) can analyze it.

These tools emit clean, structured output (JSON/CSV) suitable for piping into LLM context, notebooks, dashboards, or your own data pipelines.

## Tools

- [crono-export-cli](https://github.com/quantcli/crono-export-cli) — export from Crono (nutrition, biometrics, exercise)
- [liftoff-export-cli](https://github.com/quantcli/liftoff-export-cli) — export from Liftoff (workouts, bodyweight)
- [withings-export-cli](https://github.com/quantcli/withings-export-cli) — export from Withings (weight, body composition)
- [homebrew-tap](https://github.com/quantcli/homebrew-tap) — Homebrew formulas for the CLIs

## Install

```sh
brew tap quantcli/tap
brew install <tool-name>
```
