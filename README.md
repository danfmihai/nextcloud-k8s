# Nextcloud Install in kubernets cluster

## Will install Nexcloud in Kubernetes

## Prerequisites
- Kubernetes 1.9+
- PV provisioner support (nfs-client provisioner) 

1. Creates a new namespace: nextcloud
2. Setup a volume to store our NextCloud data:
 -  Deploy the Persistent Volume (PV) - dynamically with nfs client provisioner
 -  Create the Persistent Volume Claim (PVC) 
3. Creates Nextcloud DB service deployment and service
4. Creates a secret for the DB user, DB password
5. Creates the Nextcloud deployment server and service
6. Creates an ingress service to access the server from outside

