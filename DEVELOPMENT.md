## 起動手順

```bash
docker compose up -d
./tools/fresh-table
cd ruby
bundle install
DB_HOST=localhost DB_PORT=3306 DB_USER=isucon DP_PASS=isucon DB_NAME=isucon2021_prior bundle exec puma -p 7000
```

## 動作確認

```bash
curl http://localhost:7000/api/schedules
```
