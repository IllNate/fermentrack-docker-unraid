# Fermentrack Unraid docker
This is a fork of the [fermentrack-docker-pi](https://github.com/travisbaker/fermentrack-docker-pi) which was a fork of the image created by [sard0k](https://hub.docker.com/u/sard0k) for running on raspbian.

Installs Fermentrack and its prerequisites. Fermentrack is built from https://github.com/thorrak/fermentrack.

To run use:
```
docker run -d \
  -p 8890:80 \
  --name=fermentrack\
  -v <local_data_location>:/home/fermentrack/fermentrack/data \
  -v <local_data_location>/db.sqlite3:/home/fermentrack/fermentrack/db.sqlite3 \
  fermentrack-docker-unraid
```
or use the provided docker-compose.yml file to configure, then run your fermentrack image

`docker-compose up -d --force-recreate`

# UNRAID Settings


