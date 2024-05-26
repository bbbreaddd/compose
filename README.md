# Docker Compose Files
This is a repo containing the docker-compose.yml files I use for my server.
- Most files will have a label to autoupdate with watchtower
- `example.env` files will have only what I consider the most important variables, like password, config directory, and domain.
- `DATA_PATH` is where the data for the container will be stored at. (ex. `/docker/data`) Don't include a slash at the end.
- Ports will usually be randomized
