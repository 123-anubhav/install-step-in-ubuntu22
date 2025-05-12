
### ✅ 2. MongoDB Server + Client Installation Guide

This guide will help you install **MongoDB Server 7.0** and the **MongoDB shell client (`mongosh`)** on **Ubuntu Jammy (22.04)**.

---

#### 📥 Step 1: Add MongoDB GPG Key and Repository

```bash
curl -fsSL https://pgp.mongodb.com/server-7.0.asc | sudo gpg -o /usr/share/keyrings/mongodb-server-7.0.gpg --dearmor
```

```bash
echo "deb [ signed-by=/usr/share/keyrings/mongodb-server-7.0.gpg ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/7.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-7.0.list
```

---

#### 🔄 Step 2: Update Package Index

```bash
sudo apt update
```

---

#### 📦 Step 3: Install MongoDB

```bash
sudo apt install -y mongodb-org
```

---

#### ▶️ Step 4: Start and Enable MongoDB Service

```bash
sudo systemctl start mongod
sudo systemctl enable mongod
```

✅ Check MongoDB status (optional):

```bash
sudo systemctl status mongod
```

---

#### 💻 Step 5: Launch MongoDB Shell Client

```bash
mongosh
```

You’re now connected to MongoDB and ready to run commands!
