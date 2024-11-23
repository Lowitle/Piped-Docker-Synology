# Piped-Docker
## Setting up Piped-Docker on a Synology NAS

Based on https://piped-docs.kavin.rocks/docs/self-hosting/#docker-compose-nginx-aio-script

I also used some of the steps in this guide by Marius: https://mariushosting.com/how-to-install-piped-on-your-synology-nas/

1. Follow this guide from step 1 to step 18. After step 18, return to this guide. https://mariushosting.com/how-to-install-piped-on-your-synology-nas/
2. After following those steps, you'll have 3 reverse proxies: 
    - **frontend:** piped.yourname.synology.me
    - **backend:** pipedapi.yourname.synology.me
    - **proxy:** pipedproxy.yourname.synology.me
3. Now you'll need to access your synology NAS using SSH, if you don't know how, you can use this guide to know how to: https://mariushosting.com/how-to-ssh-into-a-synology-nas/
4. Run ```cd /volume1/docker```
5. Run ```git clone https://github.com/Lowitle/Piped-Docker-Synology```
6. Run ```cd Piped-Docker-Synology```
7. Run ```./configure-instance.sh``` answer the questions with the correct reverse proxy we created.
8. Run ```mkdir data```
9. Run ```mkdir data/db```
10. Run ```sudo docker-compose up -d```
11. Wait till all the containers started and then go to ```piped.yourname.synology.me```
