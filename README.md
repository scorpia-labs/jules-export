# jules-export: list and download Google Jules sessions

`jules-export` is a command-line tool that uses the [Google Jules API](https://developers.google.com/jules/api/reference/rest) to list and fetch sessions.  It is a read-only tool that does not provide access to the POST endpoints.

The tool writes JSON output to stdout.

## Usage:

List sessions:

```
jules-export [-k FILE] [-s DATE] [-e DATE] list
```

Get a specific session:

```
jules-export [-k FILE] get SESSION
```

## Command-line options

*  `-k FILE`, `--api-key-file FILE`: Location to the Jules API key file.
   Default: `$HOME/.config/jules/api-key`.
*  `-s DATE`, `--start DATE`: Limit the earliest date in the `list` output to
   the specified date (format: `YYYY-MM-DD`). Default is to not limit by date.
*  `-e DATE`, `--end DATE`: Limit the latest date in the `list` output to
   the specified date (format: `YYYY-MM-DD`). Default is to not limit by date.
