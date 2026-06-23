# Essential Linux Commands

## 1. File and Directory Management

* `ls` – List directory contents
* `cd` – Change directory
* `pwd` – Print working directory
* `cp` – Copy files and directories
* `mv` – Move or rename files and directories
* `rm` – Remove files or directories
* `mkdir` – Make directories
* `rmdir` – Remove empty directories
* `touch` – Change file timestamps or create empty files
* `find` – Search for files in a directory hierarchy
* `locate` – Find files by name
* `tree` – Display directories in a tree-like format
* `chmod` – Change file permissions
* `chown` – Change file owner and group
* `chgrp` – Change group ownership
* `stat` – Display file or file system status

---

## 2. File Viewing and Editing

* `cat` – Concatenate and display file content
* `tac` – Display file content in reverse
* `more` – View file content page by page
* `less` – Scrollable file viewer
* `head` – Show first lines of a file
* `tail` – Show last lines of a file
* `nano` – Terminal text editor
* `vim / vi` – Advanced text editors
* `emacs` – Text editor
* `grep` – Search text using patterns
* `sed` – Stream editor for filtering and transforming text
* `awk` – Pattern scanning and processing language
* `cut` – Remove sections from lines
* `sort` – Sort lines of text files
* `uniq` – Remove duplicate lines

---

## 3. Process Management

* `ps` – Display running processes
* `top` – Display Linux tasks
* `htop` – Interactive process viewer
* `kill` – Terminate a process
* `killall` – Terminate processes by name
* `bg` – Resume suspended jobs in background
* `fg` – Bring jobs to foreground
* `jobs` – List active jobs
* `nice` – Run program with modified priority
* `renice` – Change process priority
* `uptime` – Show system uptime
* `time` – Measure execution time

---

## 4. Disk Management

* `df` – Show disk space usage
* `du` – Estimate file space usage
* `fdisk` – Partition manager
* `lsblk` – List block devices
* `mount` – Mount a filesystem
* `umount` – Unmount a filesystem
* `parted` – Partition manipulation tool
* `mkfs` – Create a filesystem
* `fsck` – Check and repair filesystem
* `blkid` – Display block device information

---

## 5. Networking

* `ifconfig` – Configure network interfaces
* `ip` – Modern networking utility
* `ping` – Send ICMP requests
* `netstat` – Network statistics
* `ss` – Socket statistics
* `traceroute` – Trace network route
* `nslookup` – DNS query utility
* `dig` – DNS lookup tool
* `wget` – Download files from web
* `curl` – Transfer data using URLs
* `scp` – Secure file copy
* `ssh` – Secure shell remote login
* `ftp` – File Transfer Protocol client

---

## 6. User and Group Management

* `useradd` – Add user
* `usermod` – Modify user account
* `userdel` – Delete user account
* `groupadd` – Add group
* `groupdel` – Delete group
* `passwd` – Change password
* `chage` – Change password expiry
* `whoami` – Show current user
* `who` – Show logged-in users
* `w` – Show logged-in users and activity
* `id` – Display user/group IDs
* `groups` – Show group memberships

---

## 7. System Information and Monitoring

* `uname` – Display system information
* `hostname` – Show or set hostname
* `dmesg` – Show kernel messages
* `uptime` – How long the system has been running
 `dmesg` – Boot and system messages
* `free` – Display memory usage
* `top` – Display Linux tasks
* `vmstat` – Virtual memory statistics
* `lscpu` – CPU information
* `lsusb` – List USB devices
* `lspci` – List PCI devices
* `lshw` – Hardware configuration details

---

## 8. Archiving and Compression

```bash
* tar - Archiving Files
    tar -czf archive.tar.gz /path/to/directory - Compress files using gzip
    tar -xzf archive.tar.gz - – Extract gzipped tarball
    tar -cf archive.tar /path/to/directory – Create a tarball
    tar -xf archive.tar – Extract tarball 
* zip – Package and compress files into a ZIP archive
* unzip – Extract files from a ZIP archive
* gzip – Compress files using the gzip algorithm
* gunzip – Decompress files compressed with gzip
* bzip2 – Compress files using the bzip2 algorithm
* bunzip2 – Decompress files compressed with bzip2
* xz – Compress files using the xz algorithm
* unxz – Decompress files compressed with xz
```

## 9. Package Management (Depends on Distribution)

### Debian-Based (e.g., Ubuntu)

```bash
apt-get install <package>
apt-get update
apt-get upgrade
apt-get remove <package>
```

### Red Hat-Based Systems

```bash
yum install <package>
yum update
yum remove <package>
```

### DNF

```bash
dnf install <package>
dnf update
dnf remove <package>
```

---

## 10. Service Management

### systemctl

```bash
systemctl start <service>
systemctl stop <service>
systemctl restart <service>
systemctl enable <service>
systemctl disable <service>
systemctl status <service>
```

### service

```bash
service <service> start
service <service> stop
service <service> restart
service <service> status
```

---

## 11. Scheduling Tasks

### cron

```bash
crontab -e
crontab -l
crontab -r
```

### at

```bash
at 09:00
```

### sleep

```bash
sleep 5s
```

---

## 12. File Permissions and Security

```bash
chmod 755 file.txt
chown user:group file.txt
chgrp group file.txt
umask 022
```

### ACL Commands

```bash
setfacl
getfacl
```

### sudo Management

```bash
sudo
visudo
```

---

## 13. Backup and Restore

### rsync

```bash
rsync -avz source/ destination/
rsync -avz -e ssh source/ user@remote:/destination/
```

### dd

```bash
dd if=/dev/sda of=/path/to/backup.img
dd if=/path/to/backup.img of=/dev/sda
```

---

## 14. Diagnostics and Troubleshooting

* `journalctl` – View systemd logs
* `strace` – Trace system calls
* `lsof` – List open files
* `iostat` – CPU and disk statistics
* `mpstat` – CPU statistics
* `pidstat` – Process statistics
* `watch` – Execute command repeatedly

Example:

```bash
watch -n 1 free
```

---

## 15. Networking and Remote Management

### IP Commands

```bash
ip addr
ip link
ip route
```

### Netcat

```bash
nc -l -p 1234
nc <host> <port>
```

### Firewall Commands

```bash
ufw enable
ufw allow <port>
```

### Packet Analysis

```bash
tcpdump
```

---

## 16. Text Processing Utilities

### grep

```bash
grep 'pattern' file.txt
grep -r 'pattern' /dir/
```

### sed

```bash
sed 's/old/new/g' file.txt
```

### awk

```bash
awk '{print $1}' file.txt
```

### cut

```bash
cut -d ':' -f 1 /etc/passwd
```

### sort and uniq

```bash
sort file.txt
sort file.txt | uniq
```

### tee

```bash
echo "text" | tee file.txt
```

### tr

```bash
echo "hello" | tr 'a-z' 'A-Z'
```

### wc

```bash
wc -l file.txt
wc -w file.txt
```

---

## 17. Shutdown and Reboot

```bash
shutdown -h now
shutdown -r now
shutdown -h +10
reboot
halt
poweroff
```

### init

```bash
init 0
init 6
```

---

## 18. Filesystem Management

```bash
mount /dev/sda1 /mnt
umount /mnt
fsck /dev/sda1
```

### fstab

```bash
/etc/fstab
```

---

## 19. Docker Commands

```bash
docker run <image>
docker ps
docker ps -a
docker build -t <image_name> .
docker exec -it <container_id> bash
docker stop <container_id>
docker rm <container_id>
docker logs <container_id>
docker images
docker rmi <image_name>
docker network ls
```

### Docker Compose

```bash
docker-compose up
docker-compose down
docker-compose logs
```

---

## 20. Kubernetes Commands

```bash
kubectl get pods
kubectl get nodes
kubectl get services
kubectl apply -f file.yaml
kubectl create -f file.yaml
kubectl delete -f file.yaml
kubectl logs <pod_name>
kubectl describe pod <pod_name>
```

---

## 21. Automation Tools

### Ansible

```bash
ansible all -m ping
ansible-playbook playbook.yml
ansible-playbook --check playbook.yml
```

### Terraform

```bash
terraform init
terraform plan
terraform apply
terraform destroy
terraform validate
terraform show
```

### Puppet

```bash
puppet apply manifest.pp
puppet agent --test
```

---

## 22. CI/CD Tools

### Jenkins

```bash
java -jar jenkins.war
```

Default URL:

```text
http://localhost:8080
```

### GitLab Runner

```bash
gitlab-runner register
gitlab-runner run
```

### GitHub Actions

Located in:

```text
.github/workflows/
```

---

## 23. Cloud Commands

### AWS CLI

```bash
aws configure
aws s3 cp file.txt s3://bucket-name/
aws ec2 describe-instances
```

### Azure CLI

```bash
az login
az vm list
az group create
```

### Google Cloud SDK

```bash
gcloud auth login
gcloud compute instances list
```

---

## 24. Monitoring and Logging

### Prometheus

```bash
prometheus
prometheus --config.file=<config_file>
```

### Grafana

```bash
grafana-cli plugins install <plugin-name>
```

### ELK Stack

```bash
curl -XGET 'localhost:9200/_cluster/health?pretty'
logstash -f <config_file>
```

Kibana Default URL:

```text
http://localhost:5601
```
