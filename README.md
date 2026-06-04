# Student Management（學生管理）

本專案使用 Spring Boot 開發，並使用 Docker 容器化技術來管理 MySQL 資料庫，確保開發環境的一致性。

---

## 開發環境需求

* Java 17+
* Docker & Docker Compose
* Git

---

## 本地端啟動專案

### 1. 複製環境變數範本

```bash
cp .env.example .env
```

### 2. 開啟 `.env` 設定環境變數

```bash
MYSQL_ROOT_PASSWORD=你的 root 密碼
MYSQL_DATABASE=你的資料庫名稱
```

### 3. 啟動 Docker MySQL 容器

```bash
docker-compose up -d
```

### 4. 啟動 Spring Boot

在 IDE 中點擊 Run。
應用程式啟動後，API 會運行在 http://localhost:8080。

### 5. 停止 Docker 服務

* 停止容器

  ```bash
  docker-compose down
  ```

* 清空資料

  ```bash
  docker-compose down -v
  ```

---


