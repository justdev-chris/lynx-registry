# 🐾 Lynx Registry

This repository is the **official package registry** for the [Lynx programming language](https://github.com/justdev-chris/Lynx).

It hosts Lynx packages as versioned tarballs that can be installed via `lynx install`.

---

## 📁 Structure

```

/<pkg>/<version>/package.tar.gz

```

Example:

```

/json/1.0.0/package.tar.gz
/http/0.2.1/package.tar.gz

```

---

## 📦 How to Publish

1. Set `name` and `version` in `lynx.toml`
2. Run `lynx publish`
3. Upload `<name>-<version>.tar.gz` to this repo:
   ```bash
   mkdir -p <name>/<version>
   cp <name>-<version>.tar.gz <name>/<version>/package.tar.gz
   git add .
   git commit -m "Add <name> <version>"
   git push
```

---

📥 How to Install

```bash
lynx install
```

Packages are downloaded from:

```
https://raw.githubusercontent.com/justdev-chris/lynx-registry/main/<pkg>/<version>/package.tar.gz
```

---

📚 Documentation

Full docs in docs/.

---

📄 License

MIT