# ldb

Command-line tool for finding and enriching health, wellness and healthcare businesses (studios, gyms, clinics,
dental and medical practices, pharmacies, care providers, vets) and the people who make the buying decisions there.

This repository holds the downloads only.

## Install

Mac or Linux:

```bash
curl -fsSL https://leaddb-psi.vercel.app/install.sh | sh
```

Windows (PowerShell):

```powershell
irm https://leaddb-psi.vercel.app/install.ps1 | iex
```

Or download a file from [Releases](https://github.com/fseiwoh/ldb-cli/releases) and put it on your PATH.

## Start

```bash
ldb login                      # approve a code in your browser
ldb skills install             # teach Claude Code and Codex how to use ldb
ldb count --industry dental --country GB --by city
ldb search --industry pilates --uses mindbody --min-sites 2 --limit 100
ldb enrich accounts.csv --fields email,mobile
```

Searching and counting are free. `ldb enrich` prices everything first and asks before spending credits.
Run `ldb --help` or `ldb <command> --help` for every option.
