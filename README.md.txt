Parijat CHS — Maintenance Lookup Website (static)

Files included:
- index.html  : The main website (lookup + QR modal)
- styles.css  : Styling for the page

How it works:
1. The page sends a request to your Apps Script test web app with ?flat=FlatNo
2. The Apps Script returns an HTML page which includes a JavaScript variable 'result' with the lookup data.
3. The front-end extracts that 'result' object and displays the member's dues.
4. The 'Pay Now' button shows the QR code (embedded from path /mnt/data/ParijatQRCode.jpg).

Important:
- Replace WEBAPP_URL in index.html if your test web app URL changes.
- If hosting on GitHub Pages, upload the QR image to repo root and change the image path in index.html to './ParijatQRCode.jpg'
