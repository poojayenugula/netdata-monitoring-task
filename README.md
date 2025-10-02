# Task 7: Monitor System Resources Using Netdata

## 🛠 What I Did
- Installed Docker on Amazon Linux EC2
- Ran Netdata container using Docker
- Accessed the live Netdata dashboard at port 19999
- Collected and explored real-time system metrics (CPU, memory, disk, etc.)
- Took a screenshot of the dashboard

## 📸 Screenshot

![Dashboard Screenshot](dashboard SS.png)

## 📌 Docker Command Used

```bash
docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata

