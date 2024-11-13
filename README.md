### 獲取所有資料

```bash
curl -X GET http://127.0.0.1:5000/api/footfall
```

### 獲取某日某小時的資料

```bash
curl -X GET http://127.0.0.1:5000/api/footfall/2024-07-28/14
```

### 添加某日某小時的資料

```bash
curl -X POST http://127.0.0.1:5000/api/footfall -H "Content-Type: application/json" -d '{"date": "2024-07-29", "hour": 14, "footfall": 150}'
```

### 修改某日某小時的資料

```bash
curl -X PUT http://127.0.0.1:5000/api/footfall/2024-07-28/14 -H "Content-Type: application/json" -d "{\"footfall\": 150}"
```

### 刪除某日某小時的資料

```bash
curl -X DELETE http://127.0.0.1:5000/api/footfall/2024-07-28/14
```

### 上傳檔案加到資料庫

```bash
curl -X POST http://127.0.0.1:5000/api/upload -F "file=@data.json"
```
