
#### Example Request
```bash
curl \
-X POST \
-H "Authorization: Bearer {API_KEY}" \
-H "Content-Type: application/json" \
-H "Ngrok-Version: 2" \
-d '{"metadata":"{\"environment\":\"dev\"}","description":"kinesis dev stream","format":"json","target":{"kinesis":{"auth":{"role":{"role_arn":"arn:aws:iam::123456789012:role/example"}},"stream_arn":"arn:ngrok-local:kinesis:us-east-2:123456789012:stream/mystream2"}}}' \
https://api.ngrok.com/event_destinations
