# 作業 - 3. 使用 pm2 啟動 Node.js cluster

使用 cluster mode 啟動四個 process

## pm2.json

```
{
    "name": "smms_day1-3",
    "script": "npm start",
    "instances": 4,
    "exec_mode": "cluster"
}
```

## Command

```
pm2 start pm2.json
```
