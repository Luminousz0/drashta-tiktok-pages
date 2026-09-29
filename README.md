# Drashta TikTok Pages

This repository hosts the public, non-secret portion of the Drashta TikTok
integration: app information, policy pages and the HTTPS OAuth callback.

The private local companion runs from the Drashta project:

```sh
cd /Users/ashwin/Domus/Projects/active/drashta
python3 src/publish/tiktok_local_publisher.py
```

The callback forwards the short-lived Login Kit response to that localhost-only
service. The service exchanges it with TikTok using the locally stored client
secret and never puts a token or secret in this repository.
