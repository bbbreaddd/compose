Just installed to test it, probably not gonna use it.

1. Make the ./headscale/config beforehand.
2. Get the example config from [here](https://headscale.net/ref/configuration/). You can look at my config.yaml for reference. Place it in the `./config` folder and name it `config.yaml`
3. Make sure to modify the `server_url` in the `config.yaml` to match the public address to headscale. You need to port forward 8080 or use a reverse proxy
4. Deploy the docker-compose file.
5. Check logs for errors 
```bash
docker logs --follow headscale
```
6. Create a user
```bash
docker exec -it headscale \
  headscale users create USERNAME
```

Official Setup Documentation: https://headscale.net/setup/install/container/#configure-and-run-headscale
