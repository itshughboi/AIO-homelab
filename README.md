# AIO-homelab

1. Git clone repository // git clone https://github.com/itshughboi/AIO-homelab.git
2. Disable STUB resolver for Ubuntu. **DNSStubListener=no**
```
sudo nano /etc/systemd/resolved.conf
```
3. Restart resolved service
```
      sudo systemctl restart systemd-resolved
```
5. Change permissions on acme.json
```
chmod /traefik/acme.json to 600
```
7. Enter cloudflare API token into cf-token file. This should have read/write permissions for domain
8. Fill out .env
9. Run
10. Verify Traefik got staging cettificate
11. Edit traefik.yaml and change to production certificates
12. Generate crowdsec API and put that into .env
13. Rerun
