# Task 7 – Netdata Monitoring using Docker (Rocky Linux)

## Steps followed:
1. Installed Docker on Rocky Linux
2. Started Docker service
3. Ran Netdata container
4. Accessed dashboard at http://IP:19999
5. Captured screenshots

## Commands used:
sudo dnf install -y dnf-plugins-core
sudo dnf config-manager --add-repo=https://download.docker.com/linux/centos/docker-ce.repo
sudo dnf install -y docker-ce docker-ce-cli containerd.io
sudo systemctl start docker
sudo systemctl enable docker
sudo docker run -d --name=netdata -p 19999:19999 netdata/netdata

## Screenshots included:
- Netdata dashboard
- CPU monitoring
- Network stats
