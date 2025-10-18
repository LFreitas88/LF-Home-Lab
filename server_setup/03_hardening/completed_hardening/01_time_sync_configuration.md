# Item 01 — Time Synchronization (systemd-timesyncd)

### 📁 Category
**Time Sync**

### 🧩 Description
Ensure that the system clock remains accurate by enabling automatic time synchronization using **systemd-timesyncd** (NTP).  
Accurate system time is critical for security logs, authentication mechanisms, and auditing integrity.

### ⚙️ Priority
**High**

### 🧾 Commands and Configuration
```bash
# Check current time sync status
timedatectl status

# Enable and start NTP synchronization
sudo systemctl enable systemd-timesyncd.service
sudo systemctl start systemd-timesyncd.service

# Restart if already running
sudo systemctl restart systemd-timesyncd.service

# Verify if synchronization is active
timedatectl show | grep NTPSynchronized

# Optional: view current NTP configuration
grep -i ntp /etc/systemd/timesyncd.conf

# Optional: edit to add explicit NTP servers
sudo nano /etc/systemd/timesyncd.conf
# [Time]
# NTP=time.google.com time.cloudflare.com
# FallbackNTP=0.debian.pool.ntp.org 1.debian.pool.ntp.org
sudo systemctl restart systemd-timesyncd
```

## ✅ Expected Result

```
NTPSynchronized=yes
Correct and stable time across reboots
Logs and audit timestamps consistent and accurate
```

##💡 Notes

If Docker or containers are used, maintaining accurate time on the host system is crucial, as containers inherit the host clock.

## 📊 Verification Example

```
$ timedatectl status
               Local time: Sat 2025-10-18 15:01:09 EDT
           Universal time: Sat 2025-10-18 19:01:09 UTC
                 RTC time: Sat 2025-10-18 19:01:09
                Time zone: US/Eastern (EDT, -0400)
System clock synchronized: yes
              NTP service: active
          RTC in local TZ: no
```

# ✅ Status: Completed successfully on server-lf1
