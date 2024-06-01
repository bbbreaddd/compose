Not Working (At least permissions aren't)

Homepage: https://ntfy.sh/
Github: https://github.com/binwiederhier/ntfy
Docker Image: https://hub.docker.com/r/binwiederhier/ntfy

# Setup

If you want to configure ntfy then you need to manually make the config file. I included the config file that I use as an example.
Config file is stored in `/etc/ntfy/server.yml` inside the container, which is `${DATA_PATH}/ntfy/data/server.yml` on the host.
Here are the changes I made in the config file:
  - Added my domain
  - Added the user database file
  - Denied permission to everyone to read or send any messages
  - Enabled `behind-proxy`
  - Added a cache-dir for attachments
