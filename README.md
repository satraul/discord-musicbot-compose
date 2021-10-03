# discord-musicbot-compose

## Setup

1. Copy `data/application.example.yml` to `data/application.yml` (defaults are fine)
2. Copy `data/botconfig.example.js` to `data/botconfig.js`
3. Fill:
    - `Admins`, `Token`, `ClientID`, `ClientSecret` from https://discord.com/developers/applications
    - `Spotify.ClientID`, `Spotify.ClientSecret` from https://developer.spotify.com/dashboard/applications
    - `Website` should be where the bot frontend will be hosted.
        - By default compose will expose the bot frontend at `0.0.0.0:3000`, so the address should be `http://$SERVERPUBLICIP:3000`
        - If you setup a reverse proxy to a domain, change it accordingly e.g `https://$YOURDOMAIN`
4. Run `docker-compose up -d`