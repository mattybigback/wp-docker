## Example Secret Files

This folder contains example values for the Docker secrets used by this project.

Each file represents one secret:

| File name | What it is |
| --- | --- |
| `db-name` | MySQL database name for WordPress |
| `db-usr` | MySQL username used by WordPress |
| `db-pwd` | Password for the WordPress MySQL user |
| `db-root-pwd` | Password for the MySQL root user |

## How to use these examples

1. Use the files in this folder as references only.
2. Create matching files in `../secrets/` with your real values.
3. Keep real secrets out of source control.

The compose file reads secrets from `./secrets/*` and mounts them into containers under `/run/secrets/*`.
