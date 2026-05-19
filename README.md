# gateway-service

## Docker

Build image:

```bash
docker build -t gateway-service .
```

Run container:

```bash
docker run --rm -p 8082:8082 \
	-e SERVER_PORT=8082 \
	-e APP_GATEWAY_SECRET=my-super-secret-value \
	-e CORS_ALLOWED_ORIGINS="https://nice-beach-000a6fe0f.7.azurestaticapps.net,http://localhost:5173" \
	gateway-service
```
