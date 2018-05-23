# Simple SOCKS proxy based on Dante server #

#### Prerequisites ####

| Software       | Version                 |
|----------------|-------------------------|
| Python         | version 2.7 or higher   |
| Docker engine  | version 1.10 or higher  |
| Docker Compose | version 1.6.0 or higher |

#### Usage ####

Just replace PROXY_USERNAME, PROXY_PASSWORD, PROXY_PORT, and PROXY_WORKERS values with required: 

    $ PROXY_USERNAME=proxy_user \
      PROXY_PASSWORD=pr0xy_pa$$ \
      PROXY_PORT=1080 \
      PROXY_WORKERS=10 \
      docker-compose up -d --build

Note that every worker consumes about 60 Mb of RAM. With PROXY_WORKERS=10 total usage will use about 600 Mb.
