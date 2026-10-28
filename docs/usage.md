# Usage

## Requirements

- Python 3.12
- Windows 10 or 11 (or the platform listed in the README)

## Install

1. Install Python 3.12 and pipx.
2. Install Recon with pipx install recon-osint.
3. Create a case folder for the target.
4. Run one or more modules.
5. Export the report and archive the raw responses.

## Configuration

```text
%APPDATA%\Recon\
├── config.ini
├── profiles\
└── logs\
```

- Only public data, and only where lawful.
- Case folders keep raw responses.
- Sources are pluggable.

## Commands

```text
# install
pipx install recon-osint

# run
recon user johndoe --sources all --out case-01
recon email j@example.com --breach --json
recon domain example.com --subs --tech

# report
recon report case-01 --html
```

## Uninstall

Delete the application folder and `%APPDATA%\Recon`. No services, no
drivers, no scheduled tasks are installed.