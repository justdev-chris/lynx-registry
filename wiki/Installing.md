# Installing a Package

---

## From `lynx.toml`

```toml
[dependencies]
json = "1.0.0"
```

```bash
lynx install
```

---

Via Command Line

```bash
lynx add json
```

---

Download URL

```
https://raw.githubusercontent.com/justdev-chris/lynx-registry/main/<pkg>/<version>/package.tar.gz
```

---

Installed To

```
libs/<pkg>/
```

---

Usage in Code

```lynx
KittyPort "json"
```