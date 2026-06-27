# Publishing a Package

---

## 1. Prepare Your Project

Ensure `lynx.toml` has:

```toml
[package]
name = "json"
version = "1.0.0"
```

---

2. Run Publish

```bash
lynx publish
```

This creates <name>-<version>.tar.gz.

---

3. Upload to Registry

```bash
mkdir -p <name>/<version>
cp <name>-<version>.tar.gz <name>/<version>/package.tar.gz
```

---

4. Update Index

Add entry to packages.json:

```json
"<name>": {
    "description": "Brief description",
    "versions": ["<version>"],
    "latest": "<version>"
}
```

---

5. Commit & Push

```bash
git add .
git commit -m "Add <name> <version>"
git push
```

---

✅ Done

Your package is now available for lynx install.
