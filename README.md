# AIO-homelab

1. Git clone repository // git clone https://github.com/itshughboi/AIO-homelab.git
2. Disable STUB resolver for Ubuntu
       sudo nano /etc/systemd/resolved.conf
       Change to
           DNSStubListener=no

3. Restart resolved service
      sudo systemctl restart systemd-resolved
   
5. chmod /traefik/acme.json to 600
6. Enter cloudflare API token into cf-token file. This should have read/write permissions for domain
7. Fill out .env
8. Run
9. Verify Traefik got staging cettificate
10. Edit traefik.yaml and change to production certificates
11. Generate crowdsec API and put that into .env
12. Rerun
