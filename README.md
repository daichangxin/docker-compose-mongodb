# Setup mongodb server step by step

1. create sub folders

- `data/db`
- `.docker/mongo/`

2. create keyfile

```
openssl rand -base64 756 >  .docker/mongo/keyfile.pem
```

3. up

```
docker-compose up -d
```

4. connection info

```
mongodb://root:123456@localhost:27027/?replicaSet=rs0&readPreference=primary&ssl=false&w=majority
```
