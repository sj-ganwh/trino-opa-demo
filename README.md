# trino-opa-demo

## quickstart

### Service Up

```sh
# opa
docker run -d --name opa -p 8181:8181 openpolicyagent/opa:0.69.0 run --server --addr :8181

# trino
docker run -d --name trino -v $(pwd)/trino:/etc/trino --network host trinodb/trino:463
```
