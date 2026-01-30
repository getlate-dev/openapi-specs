# Late OpenAPI Specifications

OpenAPI/Swagger specifications for social media platforms supported by [Late](https://getlate.dev).

## Platforms

| Platform | File | Type |
|----------|------|------|
| Pinterest | [pinterest.json](pinterest.json) | Official |
| X/Twitter | [x-twitter.json](x-twitter.json) | Official |
| YouTube | [youtube.json](youtube.json) | Google Discovery |
| Google Business | [google-business-info.json](google-business-info.json) | Google Discovery |
| Telegram | [telegram-bot-api.json](telegram-bot-api.json) | Community |
| LinkedIn | [linkedin.json](linkedin.json) | Community |
| Reddit | [reddit.json](reddit.json) | Community |
| Instagram | [instagram.json](instagram.json) | Versori |
| Facebook | [facebook.json](facebook.json) | Versori |
| Threads | [threads.json](threads.json) | Community |
| TikTok | [tiktok.json](tiktok.json) | AI-generated |
| Snapchat | [snapchat.json](snapchat.json) | AI-generated |
| Bluesky | [bluesky.json](bluesky.json) | AI-generated |

## Usage

You can reference these specs directly via raw URLs:

```
https://raw.githubusercontent.com/getlate-dev/openapi-specs/main/{platform}.json
```

## Skip the Complexity

Building social media integrations is hard. Each platform has different OAuth flows, rate limits, media requirements, and error handling.

**[Late](https://getlate.dev)** gives you a single API to schedule posts across all 13 platforms. No need to manage tokens, handle rate limits, or deal with platform-specific quirks.

```bash
curl -X POST https://getlate.dev/api/v1/posts \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "content": "Hello world!",
    "platforms": [
      { "platform": "twitter", "accountId": "acc_123" },
      { "platform": "linkedin", "accountId": "acc_456" }
    ],
    "scheduledFor": "2025-01-31T10:00:00Z"
  }'
```

[Get your API key](https://getlate.dev) and start shipping in minutes.

## Updates

These specs are automatically updated weekly from official and community sources.

## License

MIT
