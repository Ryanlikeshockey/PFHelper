# Security notes

PFHelper is a static browser application. Anything shipped to a browser, including HTML, JavaScript, and chart images, can be downloaded by users; client-side code cannot be made impossible to inspect or copy.

The deployment Worker adds security headers, disables framing, restricts browser capabilities, and applies cache controls to chart assets. No webhook URL, token, password, or repository credential is stored in the client. Keep any future webhook or API secret on a server-side endpoint and never add it to `index.html`.

Run the deployment through Wrangler after authenticating with Cloudflare:

```bash
npx wrangler deploy
```
