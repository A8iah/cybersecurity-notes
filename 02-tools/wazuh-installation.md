# Wazuh Installation on Kali Linux

### 1. Open Terminal in Kali 

### 2. Run the Wazuh Quickstart installer 
​```bash
curl -sO https://packages.wazuh.com/4.9/wazuh-install.sh && sudo bash ./wazuh-install.sh -a
​```

- Enter sudo password when prompted (default: `kali`)
- Installation takes 10-20 minutes

### 3. Save the credentials 
- Username: `admin`
- Password: () 

### 4. Access the Wazuh Dashboard 
Open Firefox in Kali and go to:
​```
https://localhost OR https://127.0.0.1
​```

## Useful Commands

**Check Wazuh services status**
```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```

**Start / Stop / Restart services**
```bash
sudo systemctl start wazuh-manager
sudo systemctl stop wazuh-manager
sudo systemctl restart wazuh-manager
```

**View installation log**
```bash
sudo cat /var/log/wazuh-install.log
```

**Retrieve passwords if forgotten**
```bash
sudo tar -xvf wazuh-install-files.tar wazuh-install-files/wazuh-passwords.txt
sudo cat wazuh-install-files/wazuh-passwords.txt
```
