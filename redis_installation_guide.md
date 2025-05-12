
# ✅ Redis Server + CLI Installation Guide

This guide walks you through installing Redis Server and using the Redis CLI on Ubuntu.

---

## 📦 Install Redis

Start by updating your package index and installing Redis:

```bash
sudo apt update
sudo apt install redis-server -y
```

---

## ▶️ Start and Enable Redis Server

**Correct service name is `redis-server`, not `redis`**.

```bash
sudo systemctl enable redis-server
sudo systemctl start redis-server
sudo systemctl status redis-server
```

> ⚠️ **Note:**  
> If you try enabling the service with the wrong name (`redis`), you'll see this error:

```
Failed to enable unit: Refusing to operate on alias name or linked unit file: redis.service
```

✅ Use `redis-server` instead of `redis`.

---

## 💻 Redis CLI

You can access the Redis CLI using:

```bash
redis-cli
```

If Redis is running properly, you'll see the prompt:

```
127.0.0.1:6379>
```

---

## 🎯 Summary

- ✅ Update package index  
- ✅ Install Redis Server  
- ✅ Enable and Start `redis-server`  
- ✅ Access Redis CLI using `redis-cli`

Redis is now installed and running! 🎉
