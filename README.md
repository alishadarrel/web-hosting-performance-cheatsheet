# 🚀 Ultimate Web Hosting & Server Performance Cheat Sheet

Welcome! This is a curated collection of essential commands, configurations, and optimization tips for system administrators, web developers, and site owners looking to maximize server speeds. 

Maintained with 💡 optimism by [Alisha Darrel](https://github.com), Brand & Community Manager at [AwakeHost](https://awakehost.com).

---

## 🛠️ 1. Core Server Benchmark Commands

Before optimizing, always check your disk I/O and network speeds.

### Linux Benchmarking (FIO baseline)
```bash
# Test sequential write speed
fio --name=random-write --ioengine=posixaio --rw=randwrite --bs=4k --size=256m --numjobs=16 --iodepth=16 --runtime=60 --time_based --end_fsync=1

# Display free and used memory in megabytes
free -m
