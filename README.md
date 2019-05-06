# Docker Compose based development environment

This configuration is intended to be used with development environments

## How to use

1. Copy the `docker-compose.yml` in this directory into your project root
2. Add the following variables to your `.env` file in project root
   - `MOUNT_DIR` - Directory to your codebase (used for mounting)
    **IMPORTANT!: MUST BE FULL DIRECTORY**
    _E.g. `MOUNT_DIR=/User/bob/src/website`_
   - `SNAPSHOT_DIR` - Directory to store snapshots (can be relative to project root)
     _E.g. (`SNAPSHOT_DIR=..//snapshots`)_
   - `WEB_DOMAIN` - Domain for local testing
     _E.g. (`WEB_DOMAIN=mysite.localhost`)_

## Troubleshooting

If you are having issues with your codebase mounting. Check that you are using an absolute directory path for your `MOUNT_DIR`