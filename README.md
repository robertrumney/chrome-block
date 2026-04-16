# Website Blocker Extension for Chrome
 
A minimal Chrome extension that blocks a website of your choice.
 
## Install
 
1. Clone or download this repo
2. Open `rules.json` and replace `9gag.com` with your target domain
3. Go to `chrome://extensions`
4. Enable **Developer mode**
5. Click **Load unpacked**, select this folder
## Changing the blocked site
 
In `rules.json`, edit this line:
 
```
"urlFilter": "||9gag.com"
```
 
Replace `9gag.com` with whatever domain you want to block, e.g. `||reddit.com` or `||twitter.com`.
 
The `||` prefix matches the domain and all subdomains.
