# Piped-Docker

Based on https://piped-docs.kavin.rocks/docs/self-hosting/#docker-compose-caddy-aio-script

Guide to set up on a Synology NAS with DSM:

(WORK IN PROGRESS)

    1. Reverse proxy api, proxy, piped.
    2. cd docker
    3. git clone https://github.com/Lowitle/Piped-Docker-Synology
    4. Run cd Piped-Docker-Synolog
    5. Run ./configure-instance.sh and set api, proxy and piped.
    6. Run mkdir data
    7. Run mkdir data/db
    8. Run sudo docker-compose up -d
    9. Wait till all the containers started.

    Now go to 


