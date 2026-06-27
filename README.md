# Jad Yazbeck Portfolio

Personal portfolio website for Jad Yazbeck — Senior Marketing Strategist.

Single-file HTML site (`index.html`) with no build step. All CSS and JS are inline.

**Live:** [jadyazbek89-web.github.io](https://jadyazbek89-web.github.io)

## Run Locally

```powershell
python -m http.server 8080
# Open http://localhost:8080
```

## Structure

| File | Purpose |
|------|---------|
| `index.html` | Entire site — HTML + CSS + JS |
| `index_v1_backup.html` | Backup from before 5/22/2026 revision |
| `Jad Yazbeck Resume.pdf` | Resume (linked from hero CTA) |
| `images/` | All thumbnails and brand logos |

## Deploy

Netlify: build ZIP with Python `zipfile` (not PowerShell — forward-slash paths required):

```python
import zipfile, os
with zipfile.ZipFile('jad-portfolio-netlify.zip', 'w') as z:
    for root, dirs, files in os.walk('.'):
        dirs[:] = [d for d in dirs if d not in ['.git', '__pycache__']]
        for file in files:
            path = os.path.join(root, file)
            z.write(path, path.replace('\\', '/').lstrip('./'))
```

Then drop ZIP at netlify.com/drop.
