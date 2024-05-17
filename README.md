# Homelab Configuration Notes

## Execution

Install Docker (i used [orbstack](https://orbstack.dev/)) and run
```
docker compose up -d
```
to start the containers.

## Deployments

### Calibre

Container volume is bounded to three subdirectories under `library`:

- `library/raw` will be the raw files that need to be imported into Calibre (can delete once added to Calibre)
- `library/processed` will store the processed books and their metadata in the Calibre Library
- `library/export` can be used to export book files outside the calibre container in a flat format to be used outside the container (e.g. Dropbox)
