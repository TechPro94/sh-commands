# 🧠 Quick SH Commands

Common terminal commands for troubleshooting macOS/Linux endpoints.

## 🔍 Network
```sh
ifconfig                       # Show network interfaces
ping -c 5 8.8.8.8               # Connectivity test (5 packets)
traceroute google.com           # Trace route to host
netstat -rn                      # Show routing table
sudo dscacheutil -flushcache     # Flush DNS cache (macOS)
sudo killall -HUP mDNSResponder  # Restart DNS responder (macOS)
```

## ⚡ System Health
```sh
top                             # Real-time CPU/memory usage
vm_stat                         # Virtual memory stats
df -h                           # Disk usage (human-readable)
uptime                          # System uptime and load
whoami                          # Current logged-in user
```

## 📝 Logs & Diagnostics
```sh
tail -n 100 /var/log/system.log        # Last 100 system log lines
log show --predicate 'eventType == logEvent' --last 1d  # macOS logs (24h)
```

## ⚡ Power Management
```sh
sudo shutdown -r now           # Restart immediately
sudo shutdown -h now            # Shut down immediately
sudo shutdown -h +10             # Shut down in 10 minutes
logout                           # Log out current user
```
