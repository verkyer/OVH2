# 🎯 OVH Phantom Sniper

OVH 服务器自动抢购系统

---

## 🚀 Docker 部署

### 1. 构建并启动

```bash
docker-compose up -d --build
```

### 2. 访问

**前端地址：** http://localhost:8080

---

## ⚙️ 配置

### 修改配置文件

编辑：`backend/.env`

```env
API_SECRET_KEY=123456
PORT=5000
DEBUG=false
ENABLE_API_KEY_AUTH=true
```

### 重启生效

```bash
docker-compose up -d
```

---

## 🔧 更新代码

```bash
git pull
docker-compose down
docker-compose up -d --build
```

---

## 📝 端口

- **前端：** 8080
- **后端：** 5000

---

## 🔑 首次配置

1. 访问：http://localhost:8080/settings
2. 填写"网站安全密钥"（复制 backend/.env 中的 API_SECRET_KEY）
3. 填写 OVH API 凭据
4. 保存

---

**就这么简单！** ✨
