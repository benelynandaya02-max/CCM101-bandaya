## Firewall Configuration

## 1. Allow SSH

sudo ufw allow ssh

This command allows SSH traffic so administrators can remotely manage the server.

## 2. Configure the Default Policies

sudo ufw default deny incoming
sudo ufw default allow outgoing

The first command blocks incoming connections unless a rule allows them. The second command allows outgoing connections from the server.

## 3. Enable the Firewall

sudo ufw enable
sudo ufw status verbose

These commands activate the firewall and display its status and default policies.

## 4. Allow Port 8080

sudo ufw allow 8080/tcp
sudo ufw status numbered

The first command allows incoming TCP traffic on port 8080 for the web application. The second command displays the firewall rules with numbers.

## 5. Why SSH Must Be Allowed First

If I run sudo ufw enable before sudo ufw allow ssh, SSH connections may be blocked by the firewall's default incoming deny policy, potentially locking me out of remote administration.
