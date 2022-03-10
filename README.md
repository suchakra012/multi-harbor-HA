# multi-harbor-HA

# Creating a self-signed certificate for individual harbor instances
Follow the guide as given here https://github.com/myminseok/jumpbox-setup-main/tree/main/harbor-main

# Set up harbor instances
Download the harbor binary from releases page - https://github.com/goharbor/harbor/releases
Unzip on the path /harbor
tar xzvf harbor-offline-installer-version.tgz

# add extra_hosts parameter to Harbor configuration for replication and routing between two or more harbor instances
extra_hosts:
      - "harbor1.haas-493.pez.vmware.com:10.212.128.5"
      - "harbor2.haas-493.pez.vmware.com:10.212.128.6"    
