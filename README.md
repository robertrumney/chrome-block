# Website Blocker Extension for Chrome

A minimal Chrome extension that blocks a website of your choice.

## Install

1. Clone or download this repo
2. Edit `rules.json` and `manifest.json` to set your target domain (see below)
3. Go to `chrome://extensions`
4. Enable **Developer mode**
5. Click **Load unpacked**, select this folder

## Changing the blocked site

In `rules.json`, update the `urlFilter` and `host_permissions` values:

```json
"urlFilter": "||reddit.com"
```

In `manifest.json`, update the `host_permissions` value:

```json
"host_permissions": ["*://*.reddit.com/*"]
```

Both need to match. The `||` prefix matches the domain and all subdomains, so `||reddit.com` blocks `reddit.com`, `www.reddit.com`, `old.reddit.com`, etc.
