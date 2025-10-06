
# Inventory App — SharePoint Embed Package (v3)

Files:
- `index.html` — single-file app with offline Outbox + API integration
- `inventory-db.json` — cleaned seed (keeps 6H30027317)

## Host on GitHub Pages
1) Create a repo and upload both files to the **root**.
2) Enable **Settings → Pages → Deploy from a branch** (main / root).
3) Use the published URL in the SharePoint **Embed** web part.

## Configure API (optional)
Open the app, press F12 → Console:
```js
localStorage.setItem('api.base', 'https://your-api-host.example.com');
location.reload();
```

## SharePoint Embed
If the web part asks for embed code:
```html
<iframe src="https://<yourname>.github.io/<repo>/" width="100%" style="height:80vh;border:0;" allow="camera *; clipboard-write *"></iframe>
```

If embedding is blocked, ask IT to allow your app domain in **HTML Field Security** and enable CORS on the API for your SharePoint tenant domain.
