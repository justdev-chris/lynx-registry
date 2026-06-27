# Installing a Package

---

## From `lynx.toml`

Add dependency:

```toml
[dependencies]
json = "1.0.0"
```

Then run:

```bash
lynx install
```

---

Via Command Line

```bash
lynx add json
```

This adds it to lynx.toml and runs install.

---

URL

Packages are downloaded from:

```
https://raw.githubusercontent.com/justdev-chris/lynx-registry/main/<pkg>/<version>/package.tar.gz
```

---

Extraction

Packages are extracted to:

```
libs/<pkg>/
```

---

Usage in Code

```lynx
KittyPort "json"
```
