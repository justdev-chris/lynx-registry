# Publishing a Package

---

## 1. Prepare `lynx.toml`

```toml
[package]
name = "json"
version = "1.0.0"
```

---

2. Run lynx publish

Creates <name>-<version>.tar.gz.

---

3. Upload to Registry

```bash
mkdir -p <name>/<version>
cp <name>-<version>.tar.gz <name>/<version>/package.tar.gz
```

---

4. Update packages.json

```json
"<name>": {
    "description": "...",
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

