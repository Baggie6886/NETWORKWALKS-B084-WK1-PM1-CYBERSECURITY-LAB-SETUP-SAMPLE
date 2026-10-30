# NETWORKWALKS-B084-WK1-PM1-CYBERSECURITY-LAB-SETUP-SAMPLE
Cyber- lab-setup
# Week 01: Building My Cybersecurity Home Lab

**Project:** Cybersecurity Home Lab  
**Focus:** Virtualization, Kali Linux Installation, Network Configuration and Connectivity Testing  
**Platform:** Oracle VirtualBox  
**Operating System:** Kali Linux

## 1. Project Overview

Today, I built the room where the real work will happen.

As part of my cybersecurity learning journey, I dedicated Week 1 to building and configuring my own virtual cybersecurity laboratory.

Before moving into penetration testing, network analysis and defensive security, I wanted to establish a stable and isolated environment where I could safely learn, experiment and practice.

This week was about building the foundation.

## 2. Objectives

The main objectives were to:

- Set up a functional virtualization environment.
- Install and configure Kali Linux.
- Establish a private NAT Network.
- Create a clean virtual machine snapshot.
- Configure and verify network settings.
- Test internet connectivity and DNS resolution.

## 3. Tasks Completed

- [x] Installed and configured Oracle VirtualBox.
- [x] Imported and configured Kali Linux.
- [x] Created and configured a private NAT Network.
- [x] Created a clean virtual machine snapshot.
- [x] Configured and verified Kali Linux network settings.
- [x] Tested network connectivity.
- [x] Tested DNS resolution.

<img width="1324" height="549" alt="image" src="https://github.com/user-attachments/assets/8eb77549-1fdc-43c9-ac34-655aa0eff92a" />
<img width="1354" height="543" alt="image" src="https://github.com/user-attachments/assets/56d26b0d-0587-467e-adf7-c10d1660bff5" />
<img width="1344" height="549" alt="image" src="https://github.com/user-attachments/assets/ec3fedb5-3adc-4a09-b31d-b3ed9d162929" />
<img width="1358" height="538" alt="image" src="https://github.com/user-attachments/assets/618d3e94-289b-40c9-8bc0-a816ca6dac73" />
<img width="1364" height="523" alt="image" src="https://github.com/user-attachments/assets/996932b5-07e5-4396-8391-93f9b2e351c0" />

## 4. Tools and Technologies

| Tool | Purpose |
|---|---|
| Oracle VirtualBox | Virtualization |
| Kali Linux | Cybersecurity learning environment |
| NetworkManager | Network configuration |
| nmcli | Network management through CLI |
| Linux Terminal | Command-line administration |

## 5. Practical Commands Used

### Modify network connection settings
```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
```

### Deactivate network connection
```bash
sudo nmcli connection down "Wired connection 1"
```

### Reactivate network connection
```bash
sudo nmcli connection up "Wired connection 1"
```

### Verify network devices
```bash
nmcli device status
```

### Check IP configuration
```bash
ip addr
```

### Test network connectivity
```bash
ping -c 4 8.8.8.8
```

### Test DNS resolution
```bash
ping -c 4 google.com
```

## 6. Key Learning Outcomes

This week's practical work helped me understand:

1. How virtualization provides an environment for cybersecurity practice.
2. How Kali Linux can be configured inside a virtual machine.
3. The importance of network isolation when building a lab.
4. How to manage network connections using NetworkManager.
5. How to inspect IP configuration.
6. The difference between testing IP connectivity and DNS resolution.
7. Why snapshots are useful for restoring a clean lab environment.

## 7. Challenges and Troubleshooting

One of the practical tasks involved configuring the Kali Linux network connection.

I used NetworkManager's command-line utility (`nmcli`) to modify the connection settings, deactivate the connection and reactivate it.

The commands returned successful activation messages.

This exercise reinforced the importance of troubleshooting systematically instead of randomly changing network settings.

## 8. Screenshots and Evidence

Screenshots documenting the following stages are included in the `screenshots/` directory:

- VirtualBox configuration.
- Kali Linux environment.
- NAT Network configuration.
- Network connection management.
- Connectivity and DNS testing.

## 9. What's Next?

With the virtual lab established, my next objectives are:

- Strengthen my Linux command-line skills.
- Explore networking fundamentals.
- Practice IP addressing, ports and protocols.
- Introduce Wireshark for network traffic analysis.
- Begin basic defensive security and log analysis.

Week 1 was a reminder that every practical cybersecurity skill starts with a solid foundation.

**The environment is ready. Now the real learning begins.**

---

*This project is part of my ongoing beginner cybersecurity and SOC analyst learning journey. All practical activities are conducted in my own lab or other authorized environments.*
