# Day 3 - Users, Groups, Permissions

## 📌 Objective
Learn Linux user management, group management, file permissions, SSH key generation, and sudo privileges.

---

## ✅ Tasks Completed
- Created 5 users
- Created 3 groups
- Assigned users to groups
- Configured folder permissions
- Generated SSH key pairs
- Granted sudo access to manager user

---

## 👥 Users Created
```bash
sudo useradd -m dev1
sudo useradd -m dev2
sudo useradd -m tester1
sudo useradd -m ops1
sudo useradd -m manager1
```

---

## 👨‍👩‍👧 Groups Created
```bash
sudo groupadd developers
sudo groupadd testers
sudo groupadd operations
```

---

## 🔗 Group Assignment
```bash
sudo usermod -aG developers dev1
sudo usermod -aG developers dev2
sudo usermod -aG testers tester1
sudo usermod -aG operations ops1
sudo usermod -aG sudo manager1
```

---

## 🔐 Permissions Setup
```bash
sudo mkdir -p /company/{dev,test,ops}
sudo chmod 770 /company/dev
sudo chmod 770 /company/test
sudo chmod 770 /company/ops
```

---

## 🔑 SSH Key Generation
```bash
ssh-keygen
```

Generated files:
- `~/.ssh/id_ed25519`
- `~/.ssh/id_ed25519.pub`

---

## ⭐ Result
Successfully completed Day 3 Linux administration task.
