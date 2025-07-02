# 📄 Debian Installation Report for IoT, MQTT, Kafka Course

> Students must complete all sections of this form during Debian installation and submit it upon completion.

---

## 🔧 General Information

| Title                  | Value                                               |
| -----------------------| --------------------------------------------------- |
| Full Name              | Teerajit |
| Student ID              | 6520301001 |
| Installation Date      | 2025-06-25 |


---

## 🖥️ Device Information

- 💻 **Device Model / Type**: Virtual machine
- 🧬 **Firmware Type**:  
  - [ ] UEFI  
  - [x] BIOS  
- 🏷️ **Installation Type**:  
  - [] Physical PC  
  - [x] Virtual Machine (VM)

---

## 🗂️ Custom Partitioning

| Partition     | Size   | Filesystem | Mount Point           | Notes              |
|---------------|--------|------------|------------------------|--------------------|
| `/`           | 19GB   | ext4       | `/`                    | Main partition     |
| `udev`        | 1.9GB  | tmpfs      | `/dev`                 | Device management  |
| `tmpfs`       | 392MB  | tmpfs      | `/run`                 | Runtime filesystem |
| `tmpfs`       | 2.0GB  | tmpfs      | `/dev/shm`             | Shared memory      |
| `tmpfs`       | 5.0MB  | tmpfs      | `/run/lock`            | Lock directory     |
| `tmpfs`       | 392MB  | tmpfs      | `/run/user/1000`       | User runtime dir   |

---

## 🌐 Network Configuration (Static IP)

| Title                   | Value                                               |
| ------------------------| --------------------------------------------------- |
| Network Interface Name  | ens18|
| IP Address              | 172.30.15.50 |
| Netmask                 | 255.255.255.0 |
| Gateway                 | 172.30.15.254 |
| DNS                     | 8.8.8.8 , 172.30.15.254 |

---

## 🖧 Hostname

- 🖥️ **Hostname Set**: FDT6520301001

---

## 👤 User Account

- 👨‍💻 **Username Created**: u6520301001
- 🔐 **Is a Root Password Set?**:  
  - [X] Yes  
  - [ ] No

---

## ✅ Additional Problems Notes (if any)

> _____________________________________________________________________  
> _____________________________________________________________________  
> _____________________________________________________________________

