# Vulnerable Docker Containers
- Questions contact Omar Santos

The following are the vulnerable applications included:
 - WebGoat - running on port 6661 
 - Hackazon -running on port 6662
 - Damn Vulnerable Web Application (DVWA) - running on port 6663 


docker run --name webgoat -d --restart unless-stopped -p 6661:8080 -t webgoat/webgoat-8.0
docker run --name hackazon -d --restart unless-stopped -p 6662:80 bepsoccer/all-in-one-hackazon
docker run --name dvwa --restart unless-stopped -itd -p 6663:80 vulnerables/web-dvwa
